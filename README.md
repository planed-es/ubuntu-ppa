# How to

Run the following commands to add this repository to your system. Replace `22.04` with your Ubuntu version.

```sh
wget -O- https://planed-es.github.io/ubuntu-ppa/dists/22.04/planed-source.list > /etc/apt/sources.list.d/planed-source.list
wget -O- https://planed-es.github.io/ubuntu-ppa/KEY.gpg | gpg --dearmor | tee /etc/apt/keyrings/planed-es.gpg
apt-get update
```
