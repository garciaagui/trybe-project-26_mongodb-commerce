<a name="readme-top"></a>

<h1 align="center">Projeto MongoDB Commerce 🗄️🍔</h1>

<details>
  <summary>Sumário</summary><br />
  <ol>
    <li><a href="#sobre-o-projeto">Sobre o Projeto</a></li>
    <li><a href="#tecnologias">Tecnologias</a></li>
    <li><a href="#como-executar-o-projeto">Como Executar o Projeto</a></li>
    <li><a href="#habilidades">Habilidades</a></li>
    <li><a href="#sobre-a-trybe">Sobre a Trybe</a></li>
    <li><a href="#contato">Contato</a></li>
  </ol>
</details>

## Sobre o Projeto

Projeto **26** do curso de Desenvolvimento Web da [Trybe][trybe-site-url].

O projeto MongoDB Commerce consiste em uma série de desafios para praticar a elaboração de queries e desenvolver habilidades de consulta, atualização, criação e remoção em um banco de dados não relacional (NoSQL), o **MongoDB**.

Fora utilizado um banco de dados chamado `commerce`, que contém informações sobre o cardápio da rede de fast-food McDonald's, incluindo ingredientes, valores nutricionais e dados fictícios de vendas.

<details>
  <summary><strong>🚩 Aqui você pode consultar detalhes a respeito de cada desafio.</strong></summary> </br>

> ℹ️ Os arquivos dos desafios estão no diretório `./challenges`. O arquivo do primeiro desafio é o `desafio1.js`, do segundo é o `desafio2.js` e assim por diante.

> ℹ️ No contexto do projeto, não foi necessário utilizar o comando `use commerce` antes das queries dos arquivos de desafios.

- **Desafio 1**: Retornar a quantidade de documentos inseridos na coleção `produtos`.
- **Desafio 2**: Ordernar a coleção `produtos` pela quantidade de lanches vendidos em ordem crescente, mostrando apenas o nome e a quantidade de lanches vendidos.
- **Desafio 3**: Retornar o lanche mais vendido, mostrando apenas o nome e a quantidade do lanche mais vendido.
- **Desafio 4**: Retornar os lanches que tiveram vendas maiores que 50 e menores que 100, mostrando apenas o nome e a quantidade de lanches vendidos em ordem crescente.
- **Desafio 5**: Retornar o nome, as curtidas e vendidos dos lanches que tiveram quantidade de curtidas igual a 36 ou tenham a quantidade de vendas igual a 85.
- **Desafio 6**: Retornar o nome e as curtidas dos lanches que tiveram curtidas maiores que 10 e menores que 100.
- **Desafio 7**: Retornar o nome e vendidos dos lanches que tenham sido vendidos com uma quantidade diferente de 50 e em que o campo tags não exista.
- **Desafio 8**: Deletar os lanches com menos de 50 curtidas e retorne o nome dos lanches que restaram no banco.
- **Desafio 9**: Retornar o nome de todos os lanches que possuam calorias abaixo de 500.
- **Desafio 10**: Retornar o nome de todos os lanches que tenham o percentual de proteínas maior ou igual a 30 e menor ou igual a 40.
- **Desafio 11**: Retornar o nome do produto, a quantidade de curtidas e quantos itens foram vendidos dos produtos que não sejam iguais a Big Mac e McChicken.
- **Desafio 12**: Adicionar ketchup aos ingredientes para todos os sanduíches menos o McChicken, garantindo que não haja duplicidade nos ingredientes.
- **Desafio 13**: Incluir o campo criadoPor em todos os documentos, colocando Ronald McDonald no valor desse campo.
- **Desafio 14**: Criar uma query que retorne todos os lanches que possuem picles em seus ingredientes e mostre apenas os 3 primeiros itens contidos no array valoresNutricionais.
- **Desafio 15**: Adicionar o campo avaliacao em todos os documentos da coleção e efetue alterações nesse campo.
- **Desafio 16**: Adicionar o campo ultimaModificacao com a data corrente somente no sanduíche Big Mac.
- **Desafio 17**: Retornar a quantidade total de produtos em uma nova coleção chamada resumoProdutos.
- **Desafio 18**: Incluir bacon no final da lista de ingredientes dos sanduíches Big Mac e Quarteirão com Queijo.
- **Desafio 19**: Remover o item cebola de todos os sanduíches.
- **Desafio 20**: Remover o primeiro ingrediente do sanduíche Quarteirão com Queijo.
- **Desafio 21**: Remover o último ingrediente do sanduíche Cheddar McMelt.
- **Desafio 22**: Adicionar a quantidade de vendas dos sanduíches por dia da semana.
- **Desafio 23**: Inserir os valores combo e tasty no array tags de todos os sanduíches e aproveite para deixar os valores em ordem alfabética ascendente (A a Z).
- **Desafio 24**: Ordenar em todos os documentos os valores do array valoresNutricionais pelo campo percentual de forma decrescente.
- **Desafio 25**: Adicionar o valor muito sódio ao final do array tags nos produtos em que o percentual de sódio seja maior ou igual a 40.
- **Desafio 26**: Adicionar o valor contém sódio ao final do array tags nos produtos em que o percentual de sódio seja maior do que 20 e menor do que 40.
- **Desafio 27**: Contar quantos produtos contém Mc no nome, sem considerar letras maiúsculas ou minúsculas.
- **Desafio 28**: Contar quantos produtos têm 4 ingredientes.
- **Desafio 29**: Renomeie o campo descricao para descricaoSite em todos os documentos.
- **Desafio 30**: Remover o campo curtidas do item Big Mac.
- **Desafio 31**: Retornar o nome dos sanduíches em que o número de curtidas é maior que o número de sanduíches vendidos.
- **Desafio 32**: Retornar o nome e a quantidade de vendas (vendidos) dos sanduíches em que o número de vendas é múltiplo de 5.

  </details>

<br/>

## Tecnologias

[![Docker][docker-badge]][docker-url]
[![MongoDB][mongodb-badge]][mongodb-url]

<br/>

## Como Executar o Projeto

Para rodar o projeto, siga os passos abaixo.

1. Clone o repositório;

```
git clone git@github.com:garciaagui/trybe-project-26_mongodb-commerce.git
```

2. Navegue até a raiz do projeto;

```
cd trybe-project-26_mongodb-commerce/
```

3. Instale as dependências do projeto;

```
npm install
```

4. 🐋 Caso você não tenha o MongoDB instalado localmente, é possível inicializar um container Docker utilizando o comando abaixo. Caso contrário, pode pular este item;

```
docker run -d --name=nomeDoContainer -p 27017:27017 mongo:5.0
```

5. Na raiz do projeto, execute o seguinte comando para restaurar a base de dados `commerce`.

```
DBNAME=commerce ./scripts/resetdb.sh assets/produtos
```

<br/>

## Habilidades

<ul>
  <li>Utilização de métodos e operadores de pesquisa e consulta.</li>
  <li>Utilização de métodos de páginação.</li>
  <li>Utilização do método sort() para ordenação.</li>
  <li>Utilização de operadores de comparação.</li>
  <li>Utilização de operadores lógicos.</li>
  <li>Utilização de expressões regulares (regex).</li>
  <li>Utilização de métodos e operadores de atualização.</li>
  <li>Utilização de métodos de remoção.</li>
</ul>

<br/>

## Sobre a Trybe

_"A [Trybe][trybe-site-url] é uma escola do futuro para qualquer pessoa que queira melhorar de vida e construir uma carreira de sucesso em tecnologia, onde a pessoa só paga quando conseguir um bom trabalho."_

_"O programa conta com mais de 1.500 horas de aulas presenciais e online, aborda introdução ao desenvolvimento de software, front-end, back-end, ciência da computação, engenharia de software, metodologias ágeis e habilidades comportamentais._"

<br/>

## Contato

Projeto desenvolvido por Guilherme Garcia. Seguem abaixo minhas redes sociais e meios de contato. 🤘

[![Gmail][gmail-badge]][gmail-url]
[![Linkedin][linkedin-badge]][linkedin-url]
[![GitHub][github-badge]][github-url]
[![Instagram][instagram-badge]][instagram-url]

<p align="right"><a href="#readme-top">Voltar ao topo</a></p>

<!-- MARKDOWN LINKS & IMAGES -->

[trybe-site-url]: https://www.betrybe.com/

<!-- Stacks URLs & Badges -->

[docker-badge]: https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
[docker-url]: https://www.docker.com/
[mongodb-badge]: https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white
[mongodb-url]: https://www.mongodb.com/

<!-- Contact URLs & Badges -->

[gmail-badge]: https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white
[gmail-url]: mailto:garciaguig@gmail.com
[linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url]: https://www.linkedin.com/in/garciaagui/
[github-badge]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
[github-url]: https://github.com/garciaagui
[instagram-badge]: https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white
[instagram-url]: https://www.instagram.com/garciaagui/
