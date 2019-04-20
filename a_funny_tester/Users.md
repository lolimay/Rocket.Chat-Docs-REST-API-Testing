# Users

## Create [POST]
````
curl -H "X-Auth-Token: Z9mLYailz3M8X05_ZveMH745H7CDo9B1EIYmSbzEf2E" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -H "Content-type:application/json" \
     http://localhost:3000/api/v1/users.create \
     -d '{"name": "name", "email": "email@user.tld", "password": "anypassyouwant", "username": "uniqueusername"}'
````

## CreateToken [POST]
````userId
curl -H "X-Auth-Token: 32WVaWI9-CFofAfw8bxz5DI4zDpKpXPQ5RpZxYK8c0j" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -H "Content-type:application/json" \
     http://localhost:3000/api/v1/users.createToken \
     -d '{ "userId": "dufRJtiByvXrpm2io" }'
````

````username
curl -H "X-Auth-Token: 32WVaWI9-CFofAfw8bxz5DI4zDpKpXPQ5RpZxYK8c0j" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -H "Content-type:application/json" \
     http://localhost:3000/api/v1/users.createToken \
     -d '{ "username": "test" }'
````

## User Delete [POST]
````
curl -H "X-Auth-Token: 32WVaWI9-CFofAfw8bxz5DI4zDpKpXPQ5RpZxYK8c0j" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -H "Content-type:application/json" \
     http://localhost:3000/api/v1/users.delete \
     -d '{ "username": "test" }'
````

## User Delete Own Account
````
curl -H "X-Auth-Token: e0yvuqhb33VRsLkV-DcRwlTvALCBVU4_8MuS993VZE2" \
     -H "X-User-Id: NRwp39fMEtz56gWuB" \
     -H "Content-type:application/json" \
     http://localhost:3000/api/v1/users.deleteOwnAccount \
     -d '{ "password": "62ad5ff252c9923f316ed035a51df0201c24c239b79a02d2c1e126efbc16e730" }'
````
