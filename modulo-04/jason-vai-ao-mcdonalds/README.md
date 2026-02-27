# JSON vai ao McDonald's

<div align="center">
  <img src="./json-no-mc.jpeg" alt="drawing" width="300"/>
  <p>Jason -> JSON. Sacou a piada? 😆</p>
</div>

O objetivo deste projeto é colocar em prática os conhecimentos adquiridos de:

- Funções
- Objetos JavaScript
- JSON
- Array de Objetos

>👉 Para os requisitos `1, 2 e 3`, utilize a base de dados no arquivo `src/mcDonalds.js`
>
>👉 Para os exercícios `4, 5, 6 e 7`, utilize a base de dados no arquivo `src/data.json`

## Requisitos

### 1 - Crie uma função que retorna o produto mais caro de acordo com uma categoria

Implemente a função <code>moreExpensive</code> que deverá retornar uma string contendo qual é o produto mais caro de acordo com uma categoria que será passada como parâmetro. 

A função `moreExpensive` deve receber a base de dados a ser trabalhada (`data`) e a categoria (`category`) do produto.
A função deve retornar uma string contendo o produto mais caro da seguinte forma:

>O produto mais caro é: `nome do produto`, que custa: R$`preço do produto`.

O preço do produto deverá ser apresentado contendo 2 casas decimais.

---

### 2 - Crie uma função que verifica se um determinado item já existe

Implemente a função <code>checkItem</code> que deverá retornar se um determinado item existe ou não na base de dados.

A função `checkItem` deve receber a base de dados a ser trabalhada (`data`), a categoria (`category`) do produto e o produto a ser buscado (`item`).
A função deve retornar `true` caso o produto já exista na base de dados ou `false` caso não exista.

---

### 3 - Crie uma função que adiciona um novo item caso ele ainda não exista

Implemente a função <code>addNewItem</code> que deverá adicionar um novo item caso esse item não exista na base de dados.

A função `addNewItem` deve receber a base de dados a ser trabalhada (`data`), a categoria (`category`) do produto, o produto a ser buscado (`item`) e as outras informações de um item: `price`, `ingredients` e `calories`.

- A função deve retornar o novo item caso o produto ainda não exista na base de dados;

- Caso o item não exista, ele deve ser criado e adicionado à base de dados;

- Caso o item já exista, a função deve retornar a mensagem: `O produto: "nome do produto" já existe!`

---

### 4 - Crie uma função que conta a quantidade de pessoas por gênero

Implemente a função <code>counterGender</code> que deverá contar quantas pessoas existem na base de dados por gênero.

A função `counterGender` deve receber a base de dados a ser trabalhada (`data`) e retornar a quantidade de pessoas do gênero `male` e `female`.

A função deve retornar as informações no formato de objeto conforme o exemplo:

```js
{
  male: 10,
  female: 15
}
```

---

### 5 - Crie uma função que retorna os elementos de um determinado estado

Implemente a função <code>filterState</code> que deverá retornar todos os elementos que forem de um determinado estado.

- A função `filterState` deve receber a base de dados a ser trabalhada (`data`) e o estado a ser filtrado (`state`).

- A função deve retornar um novo array contendo todos os elementos que são do estado filtrado.

---

### 6 - Crie uma função que altera a propriedade "picture"

Implemente a função <code>changePicture</code> que deverá alterar a propriedade "picture" de todos os elementos da base de dados.

- A função `changePicture` deve receber a base de dados a ser trabalhada (`data`) e o link (`link`) a ser colocado no valor atual da propriedade;

- O valor da propriedade "picture" que deve ser colocado em todos os elementos é: `https://picsum.photos/200/300`;

- A função deve retornar um novo array contendo todos os elementos transformados.

---

### 7 - Crie um função que gera um relatório

Implemente a função <code>generateReport</code> que deverá gerar um relatório em forma de objeto, de várias informações da base de dados.

- A função `generateReport` deve receber a base de dados a ser trabalhada (`data`);

- A função `generateReport` deve retornar um objeto com várias informações:
  - `totalGuests`: valor total de pessoas convidadas. O valor deve ser um `number`;
  - `totalGender`: quantidade de pessoas por gênero. O valor deve ser um `object`;
  - `avgAge`: média de idade das pessoas. O valor deve ser um `number` com 2 casas decimais;
  - `countries`: array com todos os países representados.
    - Este array não pode conter valores repetidos - Pesquise sobre `Array.includes()`;
    - Este array deve estar ordenado em ordem alfabética (A-Z) - Pesquise sobre `Array.sort()`.

Exemplo de saída:

```js
{
  totalGuests: 104,
  totalGender: {
    male: 49,
    female: 55
  },
  avgAge: 32.94,
  countries: [
      'Albania',
      'Algeria',
      'Anguilla',
      'Argentina',
      'Aruba',
      'Azerbaijan',
      'Bahrain',
      'Bangladesh',
      'Benin',
      'Bermuda',
      'Bolivia',
      'Botswana',
      'Bouvet Island',
      'Brazil',
      ...
    ]
}
```
