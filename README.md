# centos7-systemd-nginx-sclo-php72-docker
centos7 systemd nginx sclo php72 docker

# docker build test
docker build -t centos7-systemd-nginx-sclo-php72 .

# docker run test
docker run --privileged --name centos7-systemd-nginx-sclo-php72-test -v /sys/fs/cgroup:/sys/fs/cgroup:ro -p 80:80 -d centos7-systemd-nginx-sclo-php72

# stop and rm
docker stop centos7-systemd-nginx-sclo-php72-test && docker rm centos7-systemd-nginx-sclo-php72-test
