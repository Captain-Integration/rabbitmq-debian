# rabbitmq-debian
### How to install rabbitmq on debian stretch?


**Add Erlang repository as RabbitMQ runs on the Erlang runtime.**
```
$ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
$ dpkg -i erlang-solutions_1.0_all.deb
```

**Add Erlang public key to your trusted key list**
```
wget -O- https://packages.erlang-solutions.com/ubuntu/erlang_solutions.asc | apt-key add -
```

**Install Socat (for SOcket CAT)**
```
apt-get update && apt-get install -y socat
```

**Install Erlang**
```
wget http://packages.erlang-solutions.com/debian/pool/erlang-nox_19.3-1~debian~jessie_all.deb
dpkg -i erlang-nox_19.3-1~debian~jessie_all.deb 
apt-get install -f -y
```

**Install RabbitMQ server**
```
apt-get install rabbitmq-server
```
