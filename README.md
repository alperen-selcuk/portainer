# portainer

## portainer i docker üzerinde ayağa kaldırmak için öncelikle bir directory açalım ve dataları içinde tutalım daha sonra docker çalıştıralım

```
mkdir portainer

docker run -d -p 9443:9443 -p 8000:8000 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v ${PWD}/portainer:/data portainer/portainer-ce:2.17.1
```
