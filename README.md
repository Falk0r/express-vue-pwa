# express-vue-pwa

Install server in the root directory with
```bash
npm install
```
Install client in /client/ with
```bash
npm install
```
## For development
Launch the express server
```bash
npm start
```
Launch Vue client
```bash
npm run serve
```
## For Production
Build client with 
```bash
npm run build
```
Create a .htacces in /client/dist directory
```htaccess
RewriteEngine On
RewriteCond %{HTTPS} off
RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [R,L]
```