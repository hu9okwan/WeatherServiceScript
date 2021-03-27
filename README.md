# A Simple Weather Service
This service will generate a weather.txt file to the appointed script directory every hour

## How to Install
Execute the following steps in your Linux terminal:
1. Enter `git clone https://github.com/hu9okwan/acit2420_lab6.git` to clone this repository
2. Enter `cd acit2420_lab6` to go into the newly created directory
3. Configure the wthr.service file to point to the appropriate paths:
   - Enter `vim wthr.service` to edit the file
   - Change `ExecStart=/home/vagrant/week11/wthr` to the absolute path of the wthr file
   - Change `WorkingDirectory=/home/vagrant/week11` to the absolute path of the directory where wthr is located
4. Enter `sudo mv wthr.* /etc/systemd/system` to move wthr.service and wthr.timer files
5. Enter `sudo systemctl daemon-reload` to reload the systemd manager configuration
6. Enter `sudo systemctl enable --now wthr.service` and `sudo systemctl enable --now wthr.timer` to enable this service at boot and start it immediately

Enter `cat weather.txt` while in the directory where wthr is located to display weather information
