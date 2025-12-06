# Login API

## Overview 

The Login API authenticates a user by validating their valid credentials and returns a session token upon success 


## Endpoint 

**POST** `/api/login`

## Reqest  

| Field  | Type   | Required | Description          |
|--------|--------|----------|----------------------|
|username| string | Yes      | User's login name    |
|password| string | Yes      | User's login password|

**Example Request:**

```json
{
 "username": "testuser"
 "password": "passwprd123"
}
```


## Response codes

**200 OK** : Login Sucessfull 


**401 Unauthorized** : Login failed due to invalid credentials


## Token 

On Sucessfull Login, the API returns a valid token.
This token is valid for subsequent requests untill it expres

