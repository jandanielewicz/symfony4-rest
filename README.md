* Register a new user account

```http request
POST /register
    ?username={}
    &firstname={}
    &lastname={}
    &password={}
Content-Type: application/json

HTTP1/1 200 OK
Content-Type: application/json
user: {}
```

* Login with the new account
```http request
POST /login
    ?email={}
    &password={}
Content-Type: application/json

HTTP1/1 200 OK
Content-Type: application/json
token: {}
expiresIn: {}

```

* Use this generate token for accessing resources
```http request
GET /user
X-Auth-Token: {}

HTTP1/1 200 OK
Content-Type: application/json
user: {}
```
