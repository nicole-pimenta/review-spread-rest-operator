## Diferença entre parâmetro e argumentos

> Parâmetro - A partir da definição de uma função, você pode ou não receber parâmetros contendo informações que serão utilizadas dentro de uma função

```javascript
function media(x, y, z) {
  let mediaTotal = x + y + z / 3;
  return mediaTotal;
}
```

No exemplo acima - x, y e z - são parâmetros da função media

> Argumento - Seguindo o exemplo acima , quando invocamos a função media , precisamos passar três informações , exemplo (10,9,8). Isso são chamados os argumentos da funcção

```javascript
media(10, 9, 8);
```

## SPREAD OPERATOR (argumentos)

> O conceito de spread operator , significa sintaxe de espalhamento e está muito ligados ao conceitos de Imutabilidade e ao conceito de argumentos

> Imutabilidade

```javascript
const notas = [6, 9, 8];

const novasNotas = [...notas]; //criação de um novo array com os dados copiados de notas
```

```javascript
const dadosUsuarios = ["nicole@mail.com", 123, 29];

function usuario(email, senha, idade) {
  console.log(email, senha, idade);
}

usuario(...dadosUsuarios);
```

## REST OPERATOR (parametros)

```javascript
function usuario(email, senha, ...demaisDados) {
  console.log(email, senha);
  console.log(demaisDados);
}

usuario("nick@mail.com", 12345, "Nicole", 29, "mae de pet", "desenvolvedora");
```
