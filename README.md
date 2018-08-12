# Setup a GraphQL API with Sequelize and Express.js

## Instructions
Please do follow the instructions in the article published on [medium](https://medium.com/infocentric).


# apollo server 2.0
https://github.com/apollographql/apollo-server

# apollo client 2.0
https://github.com/apollographql/apollo-client


some resource
https://www.youtube.com/watch?v=kXH2dbnHYA0
https://www.youtube.com/watch?v=DNPVqK_woRQ


1)
 Too many HTTP request

2) backend2 for frontends
   Client first popularized by netfilx
  Separated endpoints for desktop, mobile, TV.

3) graphQL is actually two different things :
  specification
  query language for API

Graphql has been developped by Facebook in 2012 and open sourced in 2015. Facebook faced some issue with mobile application doing too many fetch and asking for unnecessary data.


Problem with REST API

* no specification on how to query data, e.g. ascending sorting by author name.
* transform data structure before actully we can use it
* maintain a lot a different endpoints
* load unnecessary data
* do multiple HTTP requests

Schema written in the so-called Schema Definition Language. Schema is a model for your API.

Three root types : Query, Mutation, Subscription
There are equivlent to entries point in the rest world. 
Query is equivalt to 


the args in the resolver are the args passed in the client query

Schema is a data model of data you can query.

! means that the field is required


    title: ( parent, args, { db }, info) => {
      console.log(">>>>>>>>> parent", JSON.stringify( parent));

      console.log(">>>>>>>>> field", parent.title);
      return parent.title;
    },

