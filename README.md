# JSON server

```
npm install -g json-server
```

```
json-server db.json
```

> console輸入s會自動備份當前資料庫

## json

- json-server.json 

```json
{
    "port":3020
}

}
```
- db.json

```json
{
  "posts": [
    {
      "id": 1,
      "title": "json-server",
      "author": "typicode"
    }
  ],
  "comments": [
    {
      "id": 1,
      "body": "some comment",
      "postId": 1
    }
  ],
  "profile": {
    "name": "typicode"
  }
}
```

## method

### GET 

> /posts

```json
{
    "id": 1,
    "title": "json-server",
    "author": "typicode"
}
```

### POST

> /posts

```json
{
    "id": 2,
    "title": "My test",
    "author": "10codeing"
}
```
### PUT

> /posts/2

- 修改整個內容

```json
{
    "title": "New 2",
    "author":"232423"
}
```
### PATCH

> /posts/2

- 修改部分內容

```json
{
    "title": "New 2"
}


