#Read me for skillHub

#Api endpoints for users login 

Request : 
POST : {{domain}}/v1/customers/users

Body : {
    "email": "kingstonboysagar@gmail.com",
    "firstname": "sagar",
    "lastname": "Thapa",
}

Response : 
status_code : 200
body : {
    "message": "User created successfully",
    "data": {
        "id": 1,
        "email": ".."
    }
}

in case of error:
status_code : 400
body : {
    "message": "Email already registered"
}


404 => If the endpoint is not found


POST : /api/login
body : {
    "email": "kingstonboysagar@gmail.com",
    "password": "12345$"

}

if the user doesn't exists:
response :
status_code : 400
body : {
    "message": "The user doesn't exists"
}
