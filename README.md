# A Simple Weather Service

## How to Install
Execute the following steps in your Linux terminal:
1. Enter `git clone https://github.com/hu9okwan/acit2420_lab6.git`
2. Go into the newly created directory using `cd acit2420_lab6`
3. Configure the wthr.service file to point to the appropriate absolute paths:
   - Enter `vim wthr.service`
   - Change `ExecStart=/home/vagrant/week11/wthr` to the absolute path of the wthr file
   - Change `WorkingDirectory=/home/vagrant/week11` to the directory where wthr is located
4. Enter `mv wthr.* /etc/systemd/system`

