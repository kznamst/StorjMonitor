# StorjMonitor
Sends data about your nodes to a website, there the data can be processed.

Works on linux.

Node should alreaby be installed(otherwise storjshare wouldn't work) 
### Usage

```console
git clone https://github.com/kznamst/StorjMonitor.git
cd StorjMonitor
npm install dnode
node storjMonitor.js
```
Now add a cronjob , each hour at :55
```console
env > ~/.env
crontab -e
# In cron add: 
55 * * * * node /path/to/StorjMonitor/storjMonitor.js >> /dev/null 2>&1
```
Don't forget to change the path ^

The complete json object that you can get looks like this(https://pastebin.com/ppepiuiY) Here is only one node, but there can be more.

