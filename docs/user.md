# User API Spec

##Register User API

Endpoint: POST /api/users

Request Body:

...json
{
    "username":"yus",
    "password":"rahasia",
    "name":"alyus"
}
...

Response Body Success:
...json
{
    "data":{
    "username":"yus"
    "name":"alyus"
    }
}

Response Body Error:

...json
{
    "errors":"user name already registered"
}
...

##Login User API

Endpoint:POST /api/users/login

Request Body:
...json
{
    "username":"yus",
    "password":"rahasia"
}
...

Response Body Success:

...json
{
    "data":{
        "token":"unique-token"
    }
}
...

Response Body Error:

...json
{
    "errors":"username or password wrong"
}
...

##Update User API

##Get User API

##Logout User API