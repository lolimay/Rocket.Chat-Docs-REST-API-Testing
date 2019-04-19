# Authentication

## Login [POST]
**With username**
````
curl http://localhost:3000/api/v1/login \
    -d "user=Rocke@Rocket.com&password=Rocket Cat"
````
**With email**
````
curl http://localhost:3000/api/v1/login \
    -d "user=a_funny_tester@lolimay.cn&password=a_funny_tester"
````
**With JSON**
````
curl -H "Content-type:application/json" \
      http://localhost:3000/api/v1/login \
      -d '{ "user": "a_funny_tester", "password": "a_funny_tester" }'
````

## Logout [POST]
````
curl -H "X-Auth-Token: 1x6a4xBSw0OxajeBk1A-u3aSkHgNQWGaOWUfLfJHw3e" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -X POST http://localhost:3000/api/v1/logout
````

## Me
````
curl -H "X-Auth-Token: GPPXmFtO9uK_FXkAmeuETyWdZgtfZToNOrsps7l_OUk" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     http://localhost:3000/api/v1/me
````