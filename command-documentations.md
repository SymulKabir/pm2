## PM2 Command List
 
**Install PM2**    
 ```bash
    npm install -g pm2
 ``` 
**To show all online & offline server**
 ```bash
    pm2 list
 ```
**To start server with file path**
 ```bash
    pm2 start ./filename --name ServerName 
 ```
**To start with command**
 ```bash
    pm2 start "npm run dev" --name ServerName 
 ```
 
**To start existing single server**
 ```bash
    pm2 start ServerName/ServerID 
 ```
**To start existing all server**
 ```bash
    pm2 start all 
 ```
**To restart existing single server**
 ```bash
    pm2 restart ServerName/ServerID 
 ```
**To restart existing all server**
 ```bash
    pm2 restart all 
 ```
**To show all server log**
 ```bash
    pm2 log 
 ```
**To show single server log**
 ```bash
    pm2 log ServerName/ServerID 
 ```
**To stop existing single server**
 ```bash
    pm2 stop ServerName/ServerID 
 ```
**To stop existing all server**
 ```bash
    pm2 stop all 
 ```
**To delete existing single server**
 ```bash
    pm2 delete ServerName/ServerID 
 ```
**To delete existing all server**
 ```bash
    pm2 delete all 
 ```
**To auto start all server automaticly on server startup**
 ```bash
    pm2 save
    pm2 startup systemd
    pm2 save
 ```
