# arquitetura_MVC
- Nome do projeto: Abandono zero
- Descrição: Criar um site para que possamos colocar um formulário onde o objetivo da INSPA é colotar dados para entender os motivos para o comportamento de adoção, compra e/ou abandono dos animais de estimação> A partir disso, propor ações para o controle e redução desse problema.

- Controlados:
-  Lista -> Pegar todas as perguntas e fornecer para o usuário. 
- Gravar ->  salvar informações enviadas pelo usuário em um banco de dados
- Autenticar -> serve para autenticar a identidade do usuário que estiver fazendo o login
- Procurar -> serve para busca deinformações no banco de dados
- O controladores e o views interagem da seguinte forma: o usuário vizualiza o que aparece da viwe e a partir dai toma uma decisão de qual botão selecionar. Após selecionar um botão o controller é ativado recebendo a solicitação, processa-a e toma decisões com base nela, interagindo com o Modelo para buscar ou atualizar dados. Assim o controlador seleciona a View apropriada para exibir os resultados e passa os dados necessários para ela e por fim a view aparece uma nova informação para o usuário

- 
-View: Cabeçalho -> para o usúario saber o que tem no site, imagens -> deixar o site mais visualmente bonito, botão -> para que p usuário consiga interigir com o site, texto -> para usuário saber o objetivo do site, perguntas -> fomulário com as perguntas, enviar -> para enviar as perguntas para banco de dados, respostas -> o que o usuário for responder no questionário, email -> identificação do usuário, senha -> senha da conta do ADM, tabela-> para ver os dados e dados -> respostas dos usuários 
