## Enovy squid proxy with https upgrade 


### Overview:
```
         http             proxy req   ( https rewrite )      https 
client <--------> enovy <--------------->    squid    <--------------->  Internet
```

### Usage:
- Run env:
```bash
docker-compose up
```

 - Test proxy http base routing:
```bash
curl -H "X-Target-Route: google" :8001 -i
```
