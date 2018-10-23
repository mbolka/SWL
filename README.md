Wymagany docker w wersji 18.06
```
$ docker -v
Docker version 18.06.1-ce, build e68fc7a
```
### How to use it:
```bash
git clone http://github.com/mbolka/SWL
cd SWL
docker swarm init
git checkout task/Z1
docker-compose up -d
```


Aby podłączyć się do klienta:
```bash
docker exec -it client bash
```

Następnie na kliencie
```bash
curl -x{p1|p2|p3}:3128 {URL}
```

przykład:
```bash
curl -x p2:3128 http://plan-pwr.net
```

Aby połączyć się z określoną maszyną

```bash
docker exec -it {p1|p2|p3} bash
```

np
```bash
docker exec -it p1 bash
```

Po zakończeniu zdania:
```bash
docker-compose down
```

Aby zmienić przykład:
```bash
git checkout task/{Z1/Z2/Z3/Z4}
docker-compose up -d
```
