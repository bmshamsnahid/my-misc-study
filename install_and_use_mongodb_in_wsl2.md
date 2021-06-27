notepad
uninstall or stop mongodb server from windows if exist
sudo apt-get update
sudo apt-get install mongodb -y
cd /
sudo mkdir -p data/db
sudo chown -R `id -un` data/db
sudo service mongodb start
sudo service mongodb status
mongo


resource: https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-database
	  https://dev.to/seanwelshbrown/installing-mongodb-on-windows-subsystem-for-linux-wsl-2-19m9
Another solid approach: https://blog.codonomics.com/2020/08/connect-to-mongodb-on-windows-host-from.html

restore by db tools

explorer.exe .

restrore from ubuntu
