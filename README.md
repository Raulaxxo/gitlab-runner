
docker run -it ghcr.io/actions/actions-runner:2.315.0 bash

docker compose run --rm github-runner ./config.sh --url https://github.com/Raulaxxo/KailleraServer --token AXTGHUN2OSY5AGKKPQE3DJDGB4RZ2

docker compose run --rm github-runner ./run.sh


usermod -aG docker netred
service docker restart
service docker status
docker ps
groupadd docker
chmod 666 /var/run/docker.sock

docker cp be77143c6b39:home/runer .
