<h1 align="center">
    <img alt="Rocketseat GoStack" src="https://camo.githubusercontent.com/d25397e9df01fe7882dcc1cbc96bdf052ffd7d0c/68747470733a2f2f73746f726167652e676f6f676c65617069732e636f6d2f676f6c64656e2d77696e642f626f6f7463616d702d676f737461636b2f6865616465722d6465736166696f732e706e67" width="100%" />
</h1>

<h3 align="center">
  Desafio 02: Conceitos do Node.js
</h3>

## Versão

<a href="https://nodejs.org/pt/"> NodeJS 12.16.2 </a>

## Instalação

````sh
yarn
````

## Iniciar uma API

````sh
yarn dev
````

## Usando a API

Criar um novo repositório com método POST, chame uma URL http://localhost:3333/repositories/ e informe o corpo da requisição:

Corpo da requisição:

JSON

````sh
{
	"title": "Desafio 01",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
		"NodeJS",
		"React"
	]
}
````

Ele retorna todos os projetos cadastrados e o que acabou de ser cadastrado:

JSON

````sh
{
    "id": "b5fe2f8a-32c2-44a1-89ef-7d089d21481f",
    "title": "Desafio 01",
    "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
    "techs": [
        "NodeJS",
        "React"
    ],
    "likes": 0
}
````

Buscando todos os repositórios registrados, método GET, chame um URL http://localhost:3333/repositories/

Ele retorna todos os repositórios cadastrados:

JSON

````sh
[
    {
        "id": "f6b6e9de-bd64-4306-9ca7-b18c0a2551f4",
        "title": "Desafio 01",
        "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
        "techs": [
            "NodeJS alterando",
            "React alterando"
        ],
        "likes": 3
    },
    {
        "id": "89e52368-6fa9-4b57-8046-1b4ac569b9b9",
        "title": "Desafio 02",
        "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
        "techs": [
            "NodeJS",
            "React"
        ],
        "likes": 0
    }
]
````
Alterando um repositório cadastrado de acordo com o código informado, método PUT, chame um URL http://localhost:3333/repositories/ Código do repositório


````sh
http://localhost:3333/repositories/89e52368-6fa9-4b57-8046-1b4ac569b9b9
````

Corpo da requisição:

JSON
````sh
{
	"title": "Desafio 2",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
		"NodeJS"
	]
}
````

Ele retorna todos os repositórios registrados, in:

JSON

````sh
{
	"id": "89e52368-6fa9-4b57-8046-1b4ac569b9b9",
	"title": "Desafio 02",
	"url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
	"techs": [
	    "NodeJS"
	],
	"likes": 0
}
````

Excluindo um repositório registrado de acordo com o código informado, método DELETE, chame um URL http://localhost:3333/repositories/ Código do repositório


````sh
http://localhost:3333/repositories/89e52368-6fa9-4b57-8046-1b4ac569b9b9
````

Ele retornou o código de sucesso:

````sh
200
````

Para dar like no repositório com método POST, chame uma URL http://localhost:3333/repositories/b5fe2f8a-32c2-44a1-89ef-7d089d21481f/like:

Ele retorna o repositório com o número de likes atribuidos a ele:

JSON

````sh
{
    "id": "b5fe2f8a-32c2-44a1-89ef-7d089d21481f",
    "title": "Desafio 01",
    "url": "https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs",
    "techs": [
        "NodeJS",
        "React"
    ],
    "likes": 5
}
````
## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/michelspirlandeli/bootcamp-gostack-desafios/blob/master/gostack-template-conceitos-nodejs/LICENSE) para mais detalhes.

Feito com ♥ by Michel Spirlandeli :wave:
