# systemd-watcher

- Watch health of services defined in SERVICE_LIST 
- Send notifications for every changing state (up -> down / down -> up)
  - Over Gotify
  - Maybe more in the future

## Install

```
git clone https://gitlab.com/snax44/systemd-watcher.git
cp systemd-watcher/systemd-watcher /usr/bin/
chmod 750 /usr/bin/systemd-watcher
cp systemd-watcher.service /lib/systemd/system/ 
systemctl daemon-reload
systemctl enable --now systemd-watcher
```
