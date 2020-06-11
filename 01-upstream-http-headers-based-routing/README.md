## HTTP Header base routing to upstream server 


### Overview:
```
         http          http            https
client <-----> proxy <-----> upstream <------>  Internet
```

### Usage:
- Run env:
```bash
docker-compose up
```

 - Test proxy http base routing:
```bash
curl -H "X-Target-Route: wp" :8001 -i
curl -H "X-Target-Route: google" :8001 -i
```