Relacionamentos no MongoDB
Três formas de relacionar documentos — um-para-um, um-para-muitos e muitos-para-muitos — cada uma com as duas estratégias de modelagem: embarcado (embedded) e por referência.
---
1. Um para um
Cada documento se relaciona com exatamente um outro. Embarcar funciona bem quando os dados são sempre lidos juntos; referenciar faz mais sentido quando o lado relacionado é grande ou atualizado à parte.
Embarcado
O paciente carrega seu próprio resumo de doenças dentro do mesmo documento.
```javascript
db.patients.insertOne({ name: "Jefté", age: 35, diseaseSummary: { diseases: ["cold", "broken leg"] } })
```
Por referência
Pessoa e carro vivem em coleções separadas; o carro guarda o `ObjectId` do dono.
```javascript
db.persons.insertOne({ name: "Jefté", age: 35, salary: 3000 })

db.cars.insertOne({ model: "BMW", price: 40000, owner: ObjectId('6aa9e2cee9c288ce1241317e') })
```
---
2. Um para muitos
Um documento se relaciona com vários outros. Embarcar funciona bem quando a lista tem tamanho limitado e cresce pouco; referenciar evita documentos que crescem sem limite.
Embarcado
A pergunta guarda a lista de respostas diretamente dentro do próprio documento.
```javascript
db.questionThreads.insertOne({
  creator: "Jefté",
  question: "How does that work?",
  answers: [
    { text: "Like that." },
    { text: "Thanks!" }
  ]
})
```
Por referência
Cada cidadão aponta para sua cidade através do `cityId`.
```javascript
db.cities.insertOne({ name: "New York City", coordinates: { lat: 21, lng: 55 } })

db.citizens.insertMany([
  { name: "Jefté Goes", cityId: ObjectId("5b98d6b44d01c52e1637a99f") },
  { name: "Brenno Salvador", cityId: ObjectId("5b98d6b44d01c52e1637a99f") }
])
```
---
3. Muitos para muitos
Documentos dos dois lados se relacionam com vários do outro lado. Embarcar duplica dados entre documentos; referenciar mantém uma única fonte de verdade, geralmente com um array de IDs.
Embarcado
Os pedidos do cliente são adicionados diretamente dentro do próprio documento do cliente.
```javascript
db.customers.insertOne({ name: "Jefté", age: 35 })

db.customers.updateOne({}, {
  $set: {
    orders: [{ title: "A Book", price: 12.99, quantity: 2 }]
  }
})
```
Por referência
O livro guarda um array de `ObjectId`s apontando para seus autores.
```javascript
db.authors.insertMany([
  { name: "Jorge Amado", age: 78, address: { street: "Bahia" } },
  { name: "Graciliano Ramos", age: 55, address: { stree: "Rio de Janeiro" } }
])

db.books.updateOne({}, {
  $set: {
    authors: [
      ObjectId("5b98d9e44d01c52e1637a9a6"),
      ObjectId("5b98d9e44d01c52e1637a9a7")
    ]
  }
})
```
---
Modelagem de dados · MongoDB
