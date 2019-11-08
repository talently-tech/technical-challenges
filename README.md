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

