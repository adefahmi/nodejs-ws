```
sudo certbot certonly --standalone -d example.com -d www.example.com

# copy ssl certificate to our project directory
sudo cp /etc/letsencrypt/live/example.com/fullchain.pem ssl-celt/fullchain.pem
sudo cp /etc/letsencrypt/live/example.com/privkey.pem ssl-celt/privkey.pem

node index.js
```