# Virtualmin on Docker

Virtualmin installation on Ubuntu Xenial 

```
docker run --name=hosting \
-v hosting-etc:/etc \
-v hosting-home:/home \
-v hosting-lib:/var/lib \
-v hosting-log:/var/log \
-v hosting-www:/var/www \
--hostname=server.virtualmin.host --net=host \
--privileged --restart always -d technoexpress/virtualmin
```

### Docker Hub
https://hub.docker.com/r/technoexpress/virtualmin/builds/ automatically builds the latest changes into images which can easily be pulled and ran with a simple `docker run` command. 
