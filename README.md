# haproxy example

## Prerequisite
* `lsb_release -a`
```
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 20.04.1 LTS
Release:	20.04
Codename:	focal
```
* `docker version`
```
Client: Docker Engine - Community
 Version:           19.03.14
 API version:       1.40
 Go version:        go1.13.15
 Git commit:        5eb3275d40
 Built:             Tue Dec  1 19:20:26 2020
 OS/Arch:           linux/amd64
 Experimental:      false

Server: Docker Engine - Community
 Engine:
  Version:          19.03.14
  API version:      1.40 (minimum version 1.12)
  Go version:       go1.13.15
  Git commit:       5eb3275d40
  Built:            Tue Dec  1 19:18:53 2020
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          1.3.9
  GitCommit:        ea765aba0d05254012b0b9e595e995c09186427f
 runc:
  Version:          1.0.0-rc10
  GitCommit:        dc9208a3303feef5b3839f4323d9beb36df0a9dd
 docker-init:
  Version:          0.18.0
  GitCommit:        fec3683
```
* `docker-compose version`
```
docker-compose version 1.27.4, build 40524192
docker-py version: 4.3.1
CPython version: 3.7.7
OpenSSL version: OpenSSL 1.1.0l  10 Sep 2019
```

## Get Started
* `docker-compose up -d`: turn on two services and a haproxy in front of two services
* The first time you run `curl 172.17.0.1:8080/hello` on your **host** machine:
```
hello from service1!
```
* The second time you run `curl` on your **host** machine:
```
hello from service2!
```
