# Guide to verifying your pterodactyl panel domain using discord https verification
### The .well-known folder is typically used for hosting well-known resources or metadata for your website or web application. In the context of Discord, it is used for verification purposes.
## Here are general steps to follow:
1. Navigate to the root directory of your pterodactyl project make sure you are root before or it wont work. to go root you can simple just run sudo su command 
Default pterodactly root directory is this if you followed the doc
```
cd /var/www/pterodactyl

```

2. Create a new folder called .well-known. You can do this through your file explorer or by using terminal commands. For example, in the terminal, you could run:

```
mkdir .well-known
```
3. Inside the .well-known folder, create a file called discord. Again, you can do this through your file explorer or using terminal commands. For example:

```
touch .well-known/discord
```
4. Use any file editor you have and edit the discord file you created i prefer nano for file editing, copy the contents that discord gave you and simply paste it inside the discord file then CTRL+X after that press enter if you are using nano to save the file.
```
nano /var/www/pterodactyl/.well-known/discord
```
5. Follow the step 2-3-4 on the /var/www/pterodactyl/public directory too just repeat it.
```
cd /var/www/pterodactyl/public
mkdir .well-known
touch .well-known/discord
nano /var/www/pterodactyl/.well-known/discord
```

### This should be enough after that when you press verify you should be able to verify it without a problem 
### If you are having problems verifying make sure your web server is configured to serve files from the .well-known folder. This may involve configuring your server's .htaccess file or making adjustments to your server configuration.
