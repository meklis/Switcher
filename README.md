# Switcher easy start    

## Work with proxies
Example of startup and work with proxy used docker and docker-compose.

### Startup proxies
``` 
git clone https://github.com/meklis/switcher.git
cd switcher
docker-compose up -d --build
```


### Check proxies status
```
# Show working containers
docker ps

# Show logs from telnet-proxy
docker logs telnet-proxy
```
