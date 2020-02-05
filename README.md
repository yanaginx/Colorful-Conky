# Colorful-Conky

A edited version of SimpleC-one-Conky by luizfnunes

![screenshot](https://files.catbox.moe/dwj6b6.png)

All the instruction should be included in the orignal link: https://github.com/luizfnunes/SimpleC-one-Conky
Mine included some details that hopefully ease your installation progress.

# Requirements
 + Conky installed
 + Library Curl installed (to execute the weather)
  ```
  Install Curl on Ubuntu and Debian
  > $ sudo apt update
  > $ sudo apt install curl
  Install Curl on CentOS and Fedora 
  > $ sudo yum install curl
  ```
  
# Install
Download and extract the project in your system. 
Copy the content of the folder fonts/ to the directory ~/.fonts/
`cp fonts/* ~/.fonts/`

  ```
  I used `Font manager` for this step 
  sudo apt install font-manager
  ```
  
Copy the folder SimplecOne for the directory ~/.conky/
`cp SimplecOne/ ~/.conky`

# Execute
To run the widgets enter the commands: 
For the Weather:
  `conky -q -c ~/.conky/SimplecOne/conkyrc1`
For the Clock:
  `conky -q -c ~/.conky/SimplecOne/conkyrc2`
For the System Info/Net:
  `conky -q -c ~/.conky/SimplecOne/conkyrc3`
For the System Monitor:
  `conky -q -c ~/.conky/SimplecOne/conkyrc4`
  
# Execute All
Give write permission to the start.sh file (inside the SimplecOne directory)
  `chmod +x start.sh`
Execute the file
  `sh start.sh`
  
# Stop All
Give write permission to the stop.sh file (inside the SimplecOne directory)
  `chmod +x stop.sh`
Execute the file
  `sh stop.sh`

# Recomendations
Use your graphical environment to run the file ~/.conky/SimplecOne/start.sh at startup.
  ```
  Using --Startup Application-- on Ubuntu then add a Startup program with this command:
  /bin/bash -c "sleep 5 && ~/.conky/SimplecOne/start.sh"
  ```
