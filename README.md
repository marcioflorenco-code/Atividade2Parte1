## Atividade2Parte1

### vamos responder algumas perguntas referente a primeira parte da segunda atividade !!!!


****
## Questões:


**1. Explique o que é JSON e por que ele se tornou tão popular para troca de dados
entre aplicações.**

**2. Qual a diferença fundamental entre JSON.stringify() e JSON.parse()? Dê um
exemplo prático de quando usar cada um.**

**3. Considerando a string "JavaScript é baseada em ECMA Script", quais métodos
você usaria para:**
● Verificar se contém a palavra "Script";
● Remover a palavra "JavaScript" e gerar uma nova string;
● Substituir "baseada" por "tem origem"

**4. Qual a vantagem de usar template strings (``) em vez de concatenação com +
para criar strings complexas**

****

## vamos para as respostas :

****

**R1**    JSON(JavaScript Object Notation) e um formato de texto simples e legivel para todos , sendo ela muitas vezes , usada para organizaçao e troca de informaçoes de forma estrutural , ideal para a comunicação entre diferentes sistemas, como entre um servidor e uma aplicação web , outro exemplo muito comum de ser visto e usado,é para APIs, e a comunicação entre front-end e back-end ,que precisam de uma troca de dados muitas vezes leve e eficiente entre si , por conta disso ela se tornou tão popular pois muitas vezes por ter uma linguagem facil de se entender.

um exemplo de JSON
```js
{
"idade": "22";
"nome": "Marcio";
"cidade": "guarabira";
}
```

****
**R2**   Esses dois metodos **JSON.stringify()** e **JSON.parse()** servem como coversores de dados onde :

**●JSON.stringify()** :serve para converter um objeto JavaScript para uma string JSON , e muitas vezes usado para quando queremos enviar dados para um servidor, ou, salvar dados dentro de um arquivo.

**●JSON.parse()** :ja nesse caso conseguimos converter de uma string JSON para um objeto JavaScript, onde nele temos a possibilidade de receber dados , seja de um servidor ou de onde ele estive alocado , para usar-mos no codigo.

A SEGUIR VEJA O EXEMPLO DE COMO ELAS SAO ULTILIZADAS:
```js
//objeto JavaScript
const estudante = { aluno: "Marcio", cidade: "guarabira" , curso: "TSI" }

//converter de objeto JavaScript para JSON
const JsonString =JSON.String(estudante);
console.long(JsonString);
//saida = { aluno: "Marcio", cidade: "guarabira" , curso: " }

//converter de volta para objeto
const obj = JSON.parse(JsonString);
console.log(obj.curso);
//saida =TSI
```
****
**R2** Agora vamos aplicar metodos :

**Verificar se contém a palavra "Script"**
```js
const frase = "JavaScript é baseada em ECMA Script";
frase.incluides("Script"); // true
```
**Remover a palavra "JavaScript" e gerar uma nova string**
```js
const frase = "JavaScript é baseada em ECMA Script";
const frasenova = ftase.replace("JavaScript","");
console.log(frasenova);//saida = "é baseada em ECMA Script"
```
**Substituir "baseada" por "tem origem"**
const frase = "JavaScript é baseada em ECMA Script";
const alteracao = frase.replace ("baseada","tem origem");
console.log(alteracao);//saida = JavaScript é tem origem em ECMA Script

****
