#!/bin/bash
apt-get update -y
apt-get upgrade -y 
apt-get install git wget nano speedtest-cli squid3 -y
wget wget https://raw.githubusercontent.com/dhtm15/script/master/ovinstall
chmod +x ovinstall
./ovinstall
rm ovinstall
rm -rf /etc/ssh/sshd_config
wget https://raw.githubusercontent.com/dhtm15/script/master/sshd_config -O /etc/ssh/sshd_config
wget https://raw.githubusercontent.com/dhtm15/script/master/squidconf
chmod +x squidconf
./squidconf
wget https://raw.githubusercontent.com/dhtm15/script/master/remover -O /etc/payloads
wget https://raw.githubusercontent.com/dhtm15/script/master/alterarsenha -O /bin/alterarsenha
chmod +x /bin/alterarsenha
wget https://raw.githubusercontent.com/dhtm15/script/master/criarusuario -O /bin/criarusuario
chmod +x /bin/criarusuario
wget https://raw.githubusercontent.com/dhtm15/script/master/mudardata -O /bin/mudardata
chmod +x /bin/mudardata
wget https://raw.githubusercontent.com/QualityNet/Scripts/master/remover -O /bin/remover
chmod +x /bin/remover
wget https://raw.githubusercontent.com/QualityNet/Scripts/master/ajuda -O /bin/ajuda
chmod +x /bin/ajuda
wget https://raw.githubusercontent.com/QualityNet/Scripts/master/statusvpn -O /bin/statusvpn
chmod +x /bin/statusvpn
clear
