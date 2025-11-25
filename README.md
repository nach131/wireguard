
   ```bash
   sudo wg show
   ```


Instalacion en las PI

```sh
sudo apt update && sudo apt install wireguard -y
sudo cp peer1/peer1.conf /etc/wireguard/wg0.conf
sudo chmod 600 /etc/wireguard/wg0.conf
sudo wg-quick up wg0
sudo systemctl enable wg-quick@wg0   # opcional, para que arranque solo
```


# Instala nmap si no lo tienes (una sola vez)
# En Raspberry Pi / Debian / Ubuntu:
sudo apt install nmap -y

# Comprueba que el puerto está ABIERTO en UDP:
nmap -sU -p 51820 5.224.225.87