# arquitetura_MVC
- Nome do projeto: Abandono zero
- Descrição: Criar um site para que possamos colocar um formulário onde o objetivo da INSPA é colotar dados para entender os motivos para o comportamento de adoção, compra e/ou abandono dos animais de estimação> A partir disso, propor ações para o controle e redução desse problema.
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagrama: draw.io

Modelos (Models) 
- Em forms temos todas as informações das respostas dos usuários, como Id, nome, idade...
- Login temos os dados do login do usuário da senha e email
- A relação entre eles é que esses dados são gerenciados e definem como serão armazenados e recuperados

  
- Controlados:
-  Lista -> Pegar todas as perguntas e fornecer para o usuário. 
- Gravar ->  salvar informações enviadas pelo usuário em um banco de dados
- Autenticar -> serve para autenticar a identidade do usuário que estiver fazendo o login
- Procurar -> serve para busca deinformações no banco de dados
- O controladores e o views interagem da seguinte forma: o usuário vizualiza o que aparece da viwe e a partir dai toma uma decisão de qual botão selecionar. Após selecionar um botão o controller é ativado recebendo a solicitação, processa-a e toma decisões com base nela, interagindo com o Modelo para buscar ou atualizar dados. Assim o controlador seleciona a View apropriada para exibir os resultados e passa os dados necessários para ela e por fim a view aparece uma nova informação para o usuário
- No controller, o que entra em "listar" são todas as perguntas listas para que p usuário passa escrever e o que sai são todas as suas respostas. Em "autenticar" entra os emails e senhas que o usuário tem e saí a resposta se eles estão corretos ou não. Em "procurar" entra todos as respostas dos usuários do formulário e saí todos os dados

  
- View:
-  Cabeçalho -> para o usúario saber o que tem no site
Imagens -> deixar o site mais visualmente bonito, botão -> para que p usuário consiga interigir com o site
- Texto -> para usuário saber o objetivo do site
- Perguntas -> fomulário com as perguntas
- Enviar -> para enviar as perguntas para banco de dados
- Respostas -> o que o usuário for responder no questionário
- Email -> identificação do usuário
- Senha -> senha da conta do ADM
- Tabela-> para ver os dados
- Dados -> respostas dos usuários 

Infraestrutura:
- Cliente é o usuário final da aplicação, ele que interege com o View por meio de um navegador
- Servidor é reponsável por atender às solicitações do cliente e fornece as respostas, ele que tem a lógica do controller que processa a solicitação do cliente
- Banco de dados é onde os dados da aplicação são armazenamedos, ele contém o modelo de dados (Model) que define o comprtamento dos dados da aplicação

Justifique
_ A arquitetura MCV organiza e estrutura uma aplicação para assim facilitar a manutenção e evolução do projeto
