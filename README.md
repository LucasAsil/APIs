# APIs
## API simples sobre dados de vendas. ##

Antes de mais nada para quem gosta e usa o Python, recomendo muito os vídeos do canal Hashtag Programação. Onde não só contém Python, mas também outros assuntos de tecnologia. E como me baseei em um dos vídeos para criar esse código...
Segue o link: https://www.youtube.com/channel/UCafFexaRoRylOKdzGBU6Pgg

### Resumo do código ###
Como diz acima, o código é bem simples. Resumindo ele pega um arquivo "csv" com alguns dados, em específico(vendas) e através de um site(Heroku) consigo criar minha API.

### O código ###
1. Primeiro passo é importar as biblioteca Pandas, e o framework Flask.

![import_1](https://user-images.githubusercontent.com/68728828/147696906-9c07c8da-7684-48fe-8e9c-76367ca9d33c.jpg)

![import_2](https://user-images.githubusercontent.com/68728828/147696914-3835b6e2-fd89-4a7d-b8a7-534aef6761a6.jpg)

![import_3](https://user-images.githubusercontent.com/68728828/147696918-e1f86f6f-4a0e-45b8-a1a4-714663ed0cc3.jpg)

2. Em seguida se cria a funcionalidade do site com; a Homepage inicial, e a segunda, onde contem os dados das vendas. Lembrando que é necessário que o arquivo que será usado como banco de dados "csv", já tem que estar dentro da pasta do projeto.

![funcionalidade](https://user-images.githubusercontent.com/68728828/147697281-284a69ee-659b-45fd-aca9-33e14862d8fe.jpg)

E pode-se ver que existe uma função simples na pagina "vendas". Ondee ela lê os valores do arquivo soma os valores da coluna indicada e retorna um arquivo json.Então usamos um comando para rodar a API.

![rodar](https://user-images.githubusercontent.com/68728828/147697711-cd9bb081-3cc3-4700-b8ee-a3c346b8fadd.jpg)

### Colocando a API no ar ###
Por fim só resta executar o app e colocalo em um host, no caso o da Heroku.Para isso existe algumas configurações antes.

1. Criamos um arquivo de texto "Procfile" contendo "web: gunicorn api:app".

![proc](https://user-images.githubusercontent.com/68728828/147698593-3c5e4ada-bf00-4bdc-8458-f31b239ccf21.jpg)

  - Instalamos um complemento do "Procfile;
  
  ![guni](https://user-images.githubusercontent.com/68728828/147698611-47fac3be-943e-44ae-9ad0-76626ae2f51a.jpg)

2. Instalamos mais uma complemento que gerara um novo arquivo de texto "requirements", onde contém os aruqivos necessários para rodar a API.

![requirements](https://user-images.githubusercontent.com/68728828/147698624-87869805-6101-42f4-bd8c-e8b1cbf4be42.jpg)

### Heroku ###
Falta pouco para ter a sua própria API. Para isso é necessário criar uma conta no site Heroku, com um login a conta é facilmente criada, e em seguida é possível criar um novo app ou "site".

![heroku1](https://user-images.githubusercontent.com/68728828/147700047-56523d62-27c7-4be3-9154-a0e4cf52d74f.jpg)

Com isso você ira em Deploy e é so seguir as instruções do próprio site, onde é nescessario primiro ter instalado na maquina o git e heroku CLI

![dicas](https://user-images.githubusercontent.com/68728828/147700401-ff22ce59-cc4b-4b98-82e4-aad26a20cf4a.jpg)

Seguindo os passos certos não tem erro.E após dar seu primeiro push no site, você se deparar com algo parecido com isso...

![link1](https://user-images.githubusercontent.com/68728828/147700718-923b309f-09bd-43bb-b202-b1dc1657ad20.jpg)

![link2](https://user-images.githubusercontent.com/68728828/147700724-f2c9f7cb-22a6-45e8-87cf-74515e3c3167.jpg)

### Considerações ###
Existem alguns detalhes que posso ter deixado passar, mas o conteúdo mais importante está contido nessa minha experiencia que resolvi compartilhas.
Caso queira ver com mais detalhes pode ver o video sobre esse projeto no canal Hashtag Programação;

https://www.youtube.com/watch?v=WWVEymSt1iI

e também como criar um site com Flask;

https://www.youtube.com/watch?v=K2ejI4z8Mbg&t=2884s]
