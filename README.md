# docker-compose-mtproxy
With docker-compose file you can easy install telegram mtproto proxy and configure it. 

Also build in watchdog check for update telegram-proxy server and if new version come - update it and restart without any action from you.

# Install Docker and Compose

Install Docker core: https://docs.docker.com/engine/install/ubuntu/

Install via apt compose plugini (ubuntu/debian):
```
apt install docker-compose-plugin
```


# Clone repository
`git clone https://github.com/fornex-com/docker-compose-mtproxy.git`

# Edit config.env
In that file you can configure:
- TAG Value, for promote channel
- Preset SECRET, UP TO 16
- Secret count for generate, UP TO 16
- Workers count

# Change proxy port
By default, proxy start at 110 port, if you want another - edit **docker-compose.yml**:
- "**110**:443" 

# Start proxy
go to folder with that repository:

`cd docker-compose-mtproxy`

and run:

`docker compose up -d`

# Get logs and connections info
`docker compose logs`


# Stop proxy
From repository folder:

`docker compose down`


# Links
+ Telegram docker hub: https://hub.docker.com/r/telegrammessenger/proxy/
+ Source Code: https://github.com/TelegramMessenger/MTProxy
