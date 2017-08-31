# Fake REST API server

Using [`json-server`](https://github.com/typicode/json-server)


Initialize project by `npm run json:server`

Run it on `localhost:3000`

## You can do queries like:
http://localhost:3000/companies?name=Apple
http://localhost:3000/companies/1
http://localhost:3000/companies/1/users
http://localhost:3000/companies?_sort=votes&_order=asc

## You can add users by POST request (using POSTMAN, etc). For example to add a new user:
```
// Headers
{
  Content-type: application/json
}

// Body
{
	"firstName": "Elvis",
	"lastName": "Chan",
	"age": "100",
	"email": "elvis@elvis.com",
	"company": "3"
}
```

You will see that user has been added to the `users`. `"id"` has been automatically generated.
```
{
    "firstName": "Elvis",
    "lastName": "Chan",
    "age": "100",
    "email": "elvis@elvis.com",
    "company": "3",
    "id": "HJ8n8NrF-"
}
```

You can do other REST methods like PUT, DELETE, GET, etc.