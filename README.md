```
docker rm -f authproxy_site1
docker rm -f authproxy_site2
docker run --name authproxy_site1 -d -p 81:3000 -e APP_NAME=Site1 doug/authproxy_target_app
docker run --name authproxy_site2 -d -p 82:3000 -e APP_NAME=Site2 doug/authproxy_target_app
```
