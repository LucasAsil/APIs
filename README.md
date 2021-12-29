# APIs
## API simples sobre dados de vendas. ##

Anste de mais nada para quem gosta e usa o python, recomendo muito os videos do canal Hashtag Programação.Onde não só contém python, mas também outros assuntos de tecnologia.E como be baseei em um dos videos para criar esse código...
Segue o link: [https://www.youtube.com/channel/UCafFexaRoRylOKdzGBU6Pgg](url)

### Resumo do código ###
Como diz acima, o código é bem siples.Resumindo ele pega um arquivo "csv" com alguns dados, em específico(vendas) e através de um site(Heroku) consigo criar minha API.

### O código ###
1. Primeiro passo é importar as biblioteca Pandas, e o framework Flask.

![import_1](https://user-images.githubusercontent.com/68728828/147696906-9c07c8da-7684-48fe-8e9c-76367ca9d33c.jpg)

![import_2](https://user-images.githubusercontent.com/68728828/147696914-3835b6e2-fd89-4a7d-b8a7-534aef6761a6.jpg)

![import_3](https://user-images.githubusercontent.com/68728828/147696918-e1f86f6f-4a0e-45b8-a1a4-714663ed0cc3.jpg)

2. Em seguida se cria a funcionalidade do site com; a Homepage inical, e a segunda, onde contem os dados das vendas.Lembrando que é nescessário que o arquivo que será usado como banco de dados "csv", já tem que estar dentro da pasta do projeto.

![funcionalidade](https://user-images.githubusercontent.com/68728828/147697281-284a69ee-659b-45fd-aca9-33e14862d8fe.jpg)

E pode-se ver que existe uma função simples na pagina "vendas".Onde ela le os valores do arquivo soma os valores da coluna indicada e retorna um arquivo json.Então usamos um comando para rodar a API.

![rodar](https://user-images.githubusercontent.com/68728828/147697711-cd9bb081-3cc3-4700-b8ee-a3c346b8fadd.jpg)

### Colocando a API no ar ###
Por fim só resta executar o app e colocalo em um host, no caso o da Heroku.Para isso existe algumas configurações antes.

1. Criamos um arquivo de texto "Procfile" contendo "web: gunicorn api:app".

![proc](https://user-images.githubusercontent.com/68728828/147698593-3c5e4ada-bf00-4bdc-8458-f31b239ccf21.jpg)

  -Instalamos um complemento do "Procfile;
  
  ![guni](https://user-images.githubusercontent.com/68728828/147698611-47fac3be-943e-44ae-9ad0-76626ae2f51a.jpg)

2. Instalamos mais uma complemento que gerara um novo arquivo de texto "requirements", onde contém os aruqivos necessários para rodar a API.

![requirements](https://user-images.githubusercontent.com/68728828/147698624-87869805-6101-42f4-bd8c-e8b1cbf4be42.jpg)

### Heroku ###
Falta pouco para ter a sua própria API.Para isso é necessário criar uma conta no site Heroku


