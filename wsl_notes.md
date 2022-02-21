from https://docs.microsoft.com/en-us/windows/wsl/basic-commands

make sure that your wsl status is configured with wsl 2 and ubuntu 20.04 by typing
wsl --status

if wsl is not wsl 2 then 
wsl --set-default-version <version number>
  
if linux distribution no ubuntu 20.04
wsl --set-default <Distriubiton name >

check if you have the linux distro installed 
wsl --list --verbose

check what linux distros can be installed 
wsl --list --online
  
to unistall unwanted linux distribution
wsl --unregiester <Distribution name>
  
  
 ----------------------
  
 if you are in a powershell and and want to run as amdin type 
  start-process powershell -verb runas
  
  
  
  wsl -d Ubuntu-20.04 -u root
  to set new passworld
  
  
  ----
  ssh-keygen
   cat ~/.ssh/id_rsa.pub

  git clone git@repo
  
  
-----
after installing docker so that you can run docker from the temrinal
   sudo groupadd docker
   sudo usermod -aG docker $USER
  
  restart terminal or vs if using terminal there
  newgrp docker 
  
  test and see
  docker run hello-world
  
  
