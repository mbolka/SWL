How to use it:
git clone http://github.com/mbolka/SWL
cd SWL
docker swarm init
git checkout task/Z1
docker-compose up -d

Aby podłączyć się do klienta:
docker exec -it client bash

Następnie na kliencie

curl -x{p1|p2|p3}:3128 {URL}

przykład:
curl -x p2:3128 http://plan-pwr.net

Aby połączyć się z określoną maszyną

docker exec -it {p1|p2|p3} bash

np
docker exec -it p1 bash

Po zakończeniu zdania:
docker-compose down

Aby zmienić przykład:
git checkout task/{Z1/Z2/Z3/Z4}
docker-compose up -d
