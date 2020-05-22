## Event Manger 
**Technologies used :** GraphQL, MongoDB, NodeJS , expressJS

### Commands
> npm init
> npm install --save express body-parser
> npm install --save-dev nodemon
> npm start

> npm install --save express-graphql graphql

Open ```localhost:3000/graphql```
Put the below query inside  graphql  query editor
```
    query {
      events
    }

    mutation{
      createEvent(name:"Sports")
    }
```




```
mutation{
  createEvent(eventInput: {title:"title",description:"sample desc",date:"2020-05-22T04:40:39.834Z",price:9.99}){title,description}
}


query{
  events{
    _id
    date
  }
}
```