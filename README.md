# Worx Landroid package for Home Assistant
Worx Landroid package for Home Assistant based on Landroid Bridge by Heiner virtualzone
## Landroid Bridge installation
For the package to work, you need to install Landroid Bridge: https://github.com/virtualzone/landroid-bridge

I have a Raspberry Pi 3 Model B with Raspbain Stretch and Home Assistant in folder ~/pi/.homeassistant

Update Node
```ssh
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```
Then i build Landroid Bridge
```ssh
git clone https://github.com/virtualzone/landroid-bridge.git
cd landroid-bridge
npm install
```
I got a sqlite3 error here :( and need to install it

```
sudo apt-get install libsqlite3-dev
npm install sqlite3 --build-from-source --sqlite=/usr
npm run grunt
```
