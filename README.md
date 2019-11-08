# Real Technical Challenges


## Frontend 

### Junior JavaScript Developer | React - 35 min

Calendar Notes - Implement an application with which the user can add a note for a date they choose from a calendar.

### Middle JavaScript Developer | many fw | 50 min

DOM manipulation - Implement interactive form to allow editing, confirming tasks, disabling inputs and calculating statistics.

### Junior JavaScript Developer | React | 35 min
Search-Engine Application - Implement an application to search and filter products in an online shop.
 
------

## Mobile Dev

### Middle iOS Developer | Swift | 110 min
Enigma App - Build an app that encrypts and decrypts the text following the design of the enigma machine.

### Middle iOS Developer | Swift | 120 min
Book Keeper App - Initialize the Core Data Stack, including saving and generic item fetching and implement additional functionality by filling out the missing methods and fixing the UI functionality.

### Senior React Native Developer | Redux | 110 min
 Movie Store - Implement an application which allows users to buy all the movies they can imagine.
 
 -------
 
 ## Backend
 
 ### Senior C# Developer | .Net Framework | 180 min
 Tools for custom map with POI - Implement the tools for POIs search (on the map) and calculate an optimal tour route from user's favorite points. Additionaly, finish the implementation of a self-hosted WCF service which should provide this functionality.
 
 ### Junior Java Developer | Hibernate | 35 min
  Attribute Converter - Implement the missing Attribute Converter methods to correctly perform the entity mapping.
  
 ### Junior C# Developer | ASP.NET, .Net | 80 min
  Bookstore Inventory - Implement a couple of methods to manage bookstore inventory.
 
 ### Senior Java Developer | Distributed Store | 110min
 Distributed Configuration Store - caching, reflection, AOP, proxy aspects
 
 
 ----------------
 
 Python/DevOps Engineer

Hey there,

Please find below the Python coding test.

BACKEND/PYTHON CODING PROJECT:

* Backend Potential hire Project 2.0

Goals:

- demonstrate proficiency in Django/Python

- build something that scales gracefully & is easily extensible

- Write good API docs & Tests

Prompt:

As ***** expands internationally, we have a growing problem that many transportation suppliers we'd like to integrate cannot give us concrete zipcodes, cities, etc that they serve. To combat this, we'd like to be able to define custom polygons as their "service area" and we'd like for the owners of these shuttle companies to be able to define and alter their polygons whenever they want, eliminating the need for ***** employees to do this boring grunt work.

We'd like you to build a JSON REST API to help us solve this problem. Create a Github account if you do not have one already and put all of your source code on github. Your project should have API endpoints to create, update, delete, and retreive information about providers. Batch operations are not necessary except for get. A provider should contain the following information:

- Name
- Email
- Phone Number
- Language
- Currency

Once a provider is created they should be able to start defining service areas. These service areas will be geojson polygons and should be stored in the database in a way that they can be retreived and queried upon easily. There should be endpoints to create, update, delete, and get a polygon. Batch operations are not necessary except for get. A polygon should contain a name and price as well as the geojson information.

You should create an API endpoint to query this data. It should take a lat/lng pair as arguments and return a list of all polygons that include the given lat/lng. The name of the polygon, provider's name, and price should be returned for each polygon. This operation should be FAST. ***** has thousand of providers and hundreds of thousands of service areas.

All of this should be built in python/django. Use any extra libraries you think will help, choose whatever database you think is best fit for the task, and use caching as you see fit. Once you finish, write up some API docs (again using any tool you see fit) and make sure your code is well tested. Ensure that your code is clean, follows standard pep8 style (though you can use 120 characters per line) and has comments where appropriate.

Finally, deploy your code to a hosting service of your choice. ***** is built entirely on AWS, so bonus points will be awarded for use of AWS.
 
 ----------
 
 # Welcome to XXXXXXXXX.com

Please complete this guide by uploading your work to your own gitlab repository 
and doing a MR to this one. The branch must contain the readme file with the
responses using markdown and referencing to folders or files
that you need in order to solve the test.


## 1

We encourage documentation and investigation in order to have agile development.
We support RTFM and LMGTFY:

>___Create a file telling us when you last used RTFM and LMGTFY,
the OS you use and the languages you master___

**Response:** *You can see it [here](./01)*

## 2

Automation helps us to avoid human errors. Some of our systems use CI.

>___Write a program in the language of your choice that can accomplish this.
You can use Pseudocode.___
>___If you are not familiar with writing these programs, you can explain the
most representative concepts.___

**Response:** *You can see it [here](./02)*

## 3

A developer's portfolio is important to us. We ask you to upload 1 or 2 
projects of your authorship.

>___If you do not want to share the code, you can just paste some of it.___

**Response:** *You can see it [here](./03)*

## 4

>___Please, write a code or pseudocode that solves the problem in which I have a 
collection of numbers in ascending order. You need to find the matching pair 
that it is equal to a sum that its also given to you. If you make any 
assumption, let us know.___

>___Example:___
* [2,3,6,7]  sum = 9  - OK, matching pair (3,6)
* [1,3,3,7]  sum = 9  - No

* Consider recibe 1 000 000 numbers

**Response:** *You can see it [here](./04)*

## 5

"The message is in spanish."

>___4573746520657320656c20fa6c74696d6f207061736f2c20706f72206661766f722c20616772
6567616d6520616c2068616e676f75743a200d0a0d0a226d617274696e406d656e646f7a6164656c
736f6c61722e636f6d22207061726120736162657220717565206c6c656761737465206120657374
612070617274652e0d0a0d0a477261636961732c20792065737065726f20766572746520706f7220
617175ed212e___


>___U2kgbGxlZ2FzIGhhc3RhIGVzdGEgcGFydGUsIHBvciBmYXZvciwgY29tZW50YW1lbG8gY29uIHVu
IG1lbnNhamUu___

**Response:** *You can see it [here](./05)*


# All answers must be inside a docker image and the answer will be tested with a running container. Add lint and at least 01 unit test

------------------


# Running Tracking Server

## Introduction
Your company is building a social sports app that tracks the time and the distance of its users. They need your team to develop the backend application that can do the following:
1: Update user information
2: Get user information
3: Return the top N users sorted by a certain attribute
4: Return the top N fastest users
5: Find a running partner
6: Add basic authentication

1 - **Update user information**
URL `[POST, PATCH] /users/<username>`
Example: `POST /users/john`
This is an example of an update that the server needs to handle:
```json
{
  "ts": 1552475073,
  "distance": 5560,
  "time":  133910
}
```

Response example
```json
{
  "user": "john"
  "ts": 1552475073,
  "cumulative_distance": 5560
  "cumulative_time":  133910
}
```
You only need to maintain current user's cumulative distance and time count.
You don't need to care about distance and time units.

2 - **Get user information**
URL `/users/<username>`
Example: `/users/john`
Response:
```json
{
  "user": "john"
  "ts": 1552479073,
  "cumulative_distance": 15560
  "cumulative_time":  193910
}
```
`ts` represents the timestamp of the most recent update. 

3 - **Return the top N  users by certain attributes**
URL `/users/top/<attribute>?size=N`
Example: `/users/top/distance?size=3`
Response:
```json
[
}
  "user": "john"
  "ts": 1552479073,
  "cumulative_distance": 15560
  "cumulative_time":  193910
},
....,
....
]
```
`size` determines the number of users returned and it is optional. If `size` is invalid the server should return a bad request error. But if it isn't present you should return them all.
You should only allow `distance` and `time` as route variable.

4 - **Return the top N fastest users**
Edit the previous endpoint (`/users/top/<attribute>`)  to allow getting the fastest users using  `speed` as route variable.
Also, you can edit how you store your data or implement all the changes that you consider appropriate.
Response example:
```json
[
}
  "user": "john"
  "ts": 1552479073,
  "cumulative_distance": 15560,
  "cumulative_time":  193910,
  "average_speed":0.08024341189
},
....
]
```
**Note**: You don't need to round the speed.

5 - **Find a running partner**
Also, the company wants to add a feature to allow users to find the best running partners. The best runner partners are the users with a similar speed.
URL:  `/users/<username>/find-partners?size=N`
Example response
```json
[
}
  "user": "jenna"
  "ts": 1552479073,
  "cumulative_distance": 15560,
  "cumulative_time":  193910,
  "average_speed":0.08024341189
},
....
]
```
6 - **Add basic authentication**
There is going to be a private URL  `/users/<username>/private?token=$TOKEN` to fetch personal data.

The requests using `TOKEN=pq72KttXvPNZWC7zdLANzUsQYwDd5H2s` can access this endpoint and will get a `OK HTTP Status`, the request without a correct token will get an `Unauthorized HTTP Status`.

Probably the company is going to need to add more private endpoints in the future. Try to implement this authentication layer in the more generic way possible and without installing more packages.

## Problem Statement
1. Your task is to complete the backend application by implementing the API endpoints described above.
2. Handle accordingly the relevant HTTP codes
3. Use a simple in-memory store object to maintain state. For this you can use the variable named `STORE` from `views.py` file.
4. Be sure to complete all TODOs, but know not everything is explicitly tested. The tests that are visible to you are not the only ones, some tests will be tested upon submission and these test results will be visible only to the person scoring your solution.
5. Solve all the error that you may find in the code

## Running on your local environment
We recommend the use of a virtualenv but that is up to you.
We use **nosetests** to execute unit tests.
Your project will be executed with following command:
`pip install -e . && nosetests`

Write your code in the existing files to make the tests pass. Look for the TODO comments

Submit your code on the Devskiller platform. Make sure the tests pass there, too, before submitting.

## Good Luck!


------

## Intercorp retos

https://github.com/chrisocares/IntercorpRetail

https://github.com/lurrelo/Reto-Intercorp

https://github.com/FiorellaEffio/intercorp-reto

faltan los de esen


------

La última etapa de la aplicación al cargo de Sénior Technology Manager en IVisa es de demostrar tus habilidades haciendo codigo front end. En el enlace encontraras todo lo que necesitas para el challenge. El objetivo es hacer esta pequeña sección de My Wallet donde el usuario pueda adjuntar mas tarjetas, hacer la que quiera default y eliminar la que no quiera tener registrada. No es necesario que tenga header y footer (sera un plus) lo que nos importa es el modulo de cards y que este sea desarrollado en Vue.js.

https://drive.google.com/open?id=16nVLgjqVXn3AOOiVkTsSokzlSidvU8Up  

Me gustaria que la entrega este hecha en Github or Gitlab y la maqueta la podamos ver en vivo cargada en tu propio servidor. Del github la evaluacion la hace el CTO del La maqueta y sus funcionalidades nosotros.
