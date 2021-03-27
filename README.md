# A Simple Weather Service

## How to Install
Execute the following steps in your Linux terminal:
1. Enter `git clone https://github.com/hu9okwan/acit2420_lab6.git`
2. Go into the newly created directory using `cd acit2420_lab6`
3. Configure the wthr.service file to point to the appropriate absolute paths:
   - Enter `vim wthr.service`
   - Change `ExecStart=/home/vagrant/week11/wthr` to the absolute path of the wthr file
   - Change `WorkingDirectory=/home/vagrant/week11` to the absolute path of the directory where wthr is located
4. Enter `sudo mv wthr.* /etc/systemd/system`
5. Enter `sudo systemctl daemon-reload`
6. Enter `sudo systemctl enable --now wthr.service` and `sudo systemctl enable --now wthr.timer`
