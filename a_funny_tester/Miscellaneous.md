# Miscellaneous Information

## Info [GET]
````
curl http://localhost:3000/api/info
````
## Directory [GET]
````
curl -G -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
          -H "Content-type: application/json" \
          http://localhost:3000/api/v1/directory \
          --data-urlencode 'query={"text": "rocket", "type": "users", "workspace": "local"}'
````
## Shield SVG [GET]
````
curl http://localhost:3000/api/v1/shield.svg
````
## Spotlight [GET]
````
curl -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     http://localhost:3000/api/v1/spotlight?query=@root
````
## Statistics [GET]
````
curl -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     http://localhost:3000/api/v1/statistics
````
## Statistics List [GET]
````
curl -H "X-Auth-Token: BVDhOMDRZNBxhxsHkWdF526qAk_yEVZ5VrE6mD6QAv0" \
     -H "X-User-Id: 6uaRuvyJdc9jvg3Hy" \
     "http://localhost:3000/api/v1/statistics.list?query=%7B%22_id%22%3A%22v3D4mvobwfznKozH8%22%7D&fields=%7B%22os%22%3A0%2C%22migration%22%3A0%2C%22deploy%22%3A0%2C%22process%22%3A0%7D"
````