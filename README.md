# mini-wp


all endpoints is pointing to http://35.232.133.45

# Getting Started


## Register a User
### REQUEST 

```sh
[POST] /users/register
```

### BODY
```sh
username: string
email: string
password: string
```

### RESPONSE
```sh
{
    "id": 8
    "username": "username",
    "email": "useremail@mail.com"
}

```


# Getting Authenticated
Get authentication token as access key to be able to use all the features
## Signing In
Signing in with the registered username and password.
if you don't have a registered username and password, please refer to  [Register a User](#register-a-user)
### REQUEST 

```sh
[POST] /users/login
```

### BODY
```sh
username: string
password: string
```

### RESPONSE
```sh
{
    "token": "exampletoken"
}
```


Use the token generated by the logging-in response as headers to access this API's features.


