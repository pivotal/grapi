# grapi

# Start
1. `npm install`
1. make a `grapi.yml`
1. `npm start`

# Example grapi.yml
```yml
---
api_url: http://api.run.pviotal.io
```

# Example query
```
curl -X POST -H "Content-Type: application/graphql" -H "Authorization: $(cf oauth-token)" localhost:5000/graphql -d "{apps(limit: 1) {name, packages {guid, state}, processes {guid, instances, type}}}"
```
