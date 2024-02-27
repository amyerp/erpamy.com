# AMY ERP/CRM website
//test
- Production

```
docker run \
--restart=always \
-v /var/www/erpamy.com:/src \
--network="lb" \
--name  erpamy.com \
-dt klakegg/hugo \   
server --disableLiveReload \
-b="https://erpamy.com" \
--port=443

```

- Localhost
```
docker run \
--restart=always \
-v /Users/alex/Documents/git/erpamy.com-hugo:/src \
-p 7171:7171 \
--name  newerpamysite \
-dt klakegg/hugo \
server --disableLiveReload \
-b="http://localhost:7171" \
--port=7171

```
