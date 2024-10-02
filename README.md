# How to

Run the following commands to add this repository to your system. Replace `22.04` with your Ubuntu version.

```sh
wget -O- https://planed-es.github.io/ubuntu-ppa/dists/22.04/planed.list > /etc/apt/sources.list.d/planed.list
wget -O- https://planed-es.github.io/ubuntu-ppa/KEY.gpg | gpg --dearmor | tee /etc/apt/keyrings/planed-es.gpg
apt-get update
```

**Supported systems:** Ubuntu 22.04, Ubuntu 24.04
**Supported archs:** amd64



## Note for Ubuntu 22.04

Some packages need gcc>=12, so you'll have to do the following:

```sh
add-apt-repository ppa:ubuntu-toolchain-r/test
apt-get install --only-upgrade libstdc++6
```
