## Jira app

Запуск приложения
```
sail up
```

Пример запроса:
```
curl --location --request POST 'http://localhost/jira' \
--header 'Accept: application/json' \
--header 'Content-Type: application/json' \
--data-raw '{
"issue_url": "https://sample.jira-dev.com/rest/api/2/issue/11111",
"issue_id": 11111,
"fields": {
"name": "Some Name",
"content": "Some Text"
},
"created": 1645177810
}'
```

Запуск обновления команды:
```
sail artisan jira:posts-update
```