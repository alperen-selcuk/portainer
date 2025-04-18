# portainer install

portainer i docker üzerinde ayağa kaldırmak için öncelikle bir directory açalım ve dataları içinde tutalım daha sonra docker çalıştıralım

```
mkdir portainer

docker run -d -p 9443:9443 -p 8000:8000 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v ${PWD}/portainer:/data portainer/portainer-ce:2.29.0
```

9443 üsütnden eriştikten sonra admin ve password ayarlacağınız ekran gelecek.

![image](https://github.com/user-attachments/assets/bf81264c-eef7-4b51-a2ab-91cd1206b99b)
