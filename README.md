
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