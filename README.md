# TesteMagazord
Repositório criado para listar os testes feitos por mim, utilizando React Native para a Magazord

Cada um dos testes tem a finalidade de comprovar meu conhecimento em características específicas do framework.

Por questões de garantir a compatibilidade e facilidade de execução e inspeção dos testes realizados, decidi utilizar a snack.expo.dev, que é a plataforma da Expo utilizada para desenvolver utilizando o expo no próprio navegador. 

Tarefa 1:

https://snack.expo.dev/@igorceola/maga01

A listagem de tarefas é bem simples, e ao clicar sobre uma delas, eu exibo uma imagem à direita e deixo o elemento mais transparente, indicando que o mesmo está concluído. Além disso, decidi aplicar o armazenamento local usando AsyncStorage nesta tarefa como parte dos requerimentos da tarefa 5, por isso decidi fazer um cadastro de tarefas, onde é possível incluir uma tarefa e também excluir todas as tarefas existentes.

Tarefa 2:

https://snack.expo.dev/@igorceola/maga02

Nesta tarefa eu utilizei a API de https://home.openweathermap.org/ para buscar as informações de clima. Eu trago a temperatura, descrição do clima, nível de umidade e nome da cidade atual, tudo com base na geolocalização atual. Dependendo do clima registrado nos parâmetros da requisição, é mostrada um ícone diferente para melhor ilustração.  

Devo esclarecer algumas coisas:

1 - A chave da api está fixa na constante API_KEY, e espero que o número de requisições permitidas para esta chave seja suficiente ao realizarem os testes, mas caso não seja possível, para criar uma nova chave, pode-se criar uma conta em https://home.openweathermap.org/(link) e após isso acessar as informações da conta, onde se pode criar uma nova chave.

2 - No snack temos a opção de rodar a aplicação no navegador e também no próprio dispositivo móvel, lendo o qrcode exibido no Snack.expo.dev (é necessário ter o aplicativo Expo Go instalado no aparelho móvel em questão). O que ocorre é que a minha aplicação tem um pequeno erro de precisão na geolocalização quando é iniciada pela web, podendo mostrar uma cidade próxima, no lugar da atual. Neste caso, sugiro fortemente rodar a aplicação pelo aparelho móvel utilizando o qrcode, pois lá a geolocalização é feita corretamente.

Tarefa 3: 

https://snack.expo.dev/@igorceola/maga03

Decidi fazer uma loja de jogos aqui, já que é bem alinhado ao meu gosto. Utilizo React Navigation para realizar a transição entre as duas telas existentes. A listagem de produtos é bem parecida com a listagem de tarefas, da Tarefa 1. 

Tarefa 4: 

https://snack.expo.dev/@igorceola/maga04

Utilizei a própria tarefa 3 para incorporar a troca de temas, e também aproveitei para aplicar uma animação de transição de telas, já pensando no que também foi sugerido na tarefa 5. Utilizei o Theme Provider para possibilitar o gerenciamento de diferentes estilos, além de criar o arquivo ThemeContext.js que irá ajudar a fazer o controle dos dois estilos possíveis, buscando os estilos nos arquivos LightTheme.js e DarkTheme.js.

Nas telas de Listagem e Detalhe, os estilos do StyleSheet sào sobrescritos utilizando um hook com o valor vindo dos métodos do arquivo ThemeContext.js.

Além disto, adicionei um botão que exibe um menu lateral com animação, neste menu está o botão para alterar o tema da aplicação como um todo.

Considerações finais:

Espero que tudo dê certo na execução das aplicações e deixo meus agradecimentos a vocês da Magazord!
