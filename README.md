# dockerizando-sorteio

Olá! Esta é uma prática sobre alguns conceitos básicos com a tecnologia docker, o template da aplicação, como o banco de dados, as rotas, e as lógicas inclusas já foram dadas. Também não há nenhuma complexidade no que diz respeito à arquitetura, entre outras coisas. O foco é realmente fazer a build da aplicação node mediante um Dockerfile, conectá-la ao banco de dados postgres, montar um arquivo docker-compose, e fazer com que a aplicação funcione em qualquer máquina.

Entretanto, para a aplicação funcionar em sua máquina é necessário ter previamente o docker instalado. Com isso, basta utilizar o seguinte comando:

```
docker-compose up -d
```

Rotas:

A rota GET /students retorna a lista de todos os estudantes.

A rota POST /students registra uma lista de estudantes com o corpo da requisição sendo:

```json
{
  "students": [
    { "name": "Estudante 1" },
    { "name": "Estudante 2" }
    // ...
  ]
}
```

A rota /students/random retorna um dos estudantes cadastrados. Se não existir nenhum cadastrado, retorna um objeto vazio.

Caso deseje, você pode importar no seu thunder client as rotas já montadas usando o thunder-collection já colocado nesse repositório. A url padrão é localhost://5000 :).

Bons estudos!
