# Auto-Start NodeJS App by Using PM2 on Ubuntu Server Startup

 
1. **Install PM2**   
   ```bash
    npm install -g pm2
   ```

2. **Start your apps with PM2**   
   ```bash
    pm2 start /var/www/myapp/server.js --name myapp
    pm2 start "npm start" --name reactapp --cwd /var/www/reactapp
    pm2 start "npm run dev" --name api-service
   ```

3. **Save process list**   
   ```bash
    pm2 save
   ```

4. **Enable PM2 startup on reboot**   
   ```bash
    pm2 startup systemd
   ```
It will give you a command — run it, then:

5. **Save process list again**   
   ```bash
    pm2 save
   ```
6. **Remove init script via**   
   ```bash
    pm2 unstartup systemd
   ```
7. **Save process list again**   
   ```bash
    pm2 save
   ```
   
✅ Now all apps managed by PM2 will start automatically after reboot.
