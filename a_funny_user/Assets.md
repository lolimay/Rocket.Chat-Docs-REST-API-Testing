# Assets

## Set Asset
````
curl -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     -F "logo=@mylogo.jpg" \
     http://localhost:3000/api/v1/assets.setAsset
````

## Unset Asset
````
curl -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     http://localhost:3000/api/v1/assets.unsetAsset \
     -H "Content-Type:application/json" \
     -d '{ "assetName": "logo", "refreshAllClients": true}'
````