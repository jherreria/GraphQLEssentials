# GraphQLEssentials
Using GraphQL, Typescript and MondoDB for a simple app


## Setup environment
```
npm i express-graphql graphql nodemon 

npm i --save-dev @babel/cli @babel/core @babel/node @babel/preset-env
```


## Test examples
1. Tun the server on terminal:  `npm start`
2. Open GraphiQL in browser
    http://localhost:8080/graphql
3. Create the product
    ```
    mutation {
      createProduct(input: {
        name: "manzanas",
        description: "machintoche",
        price: 0.44,
        soldout: false,
        stores:[
        { store: "babilonia"}
        ]    
      }){
        name
        price
      }
    }
    ```

