# Setting Up the MySQL Server
First you should download MySQL community version from their website

Set up the Root User password

![In mac you'll scroll down system settings in order to find the MySQL section](./SettingUpMySQLServer/systemSettings.png)

You also need to set a path for SQL to use the mysql commands on Mac Terminal

Ls -al    to list all files
Look for .zshrc
Or create it with “touch .zshrc”
Then open it with “nano .zshrc” or “open .zshrc”
Add “Export Path=${PATH}:/usr/local/mysql/bin/” into the file
But actually replace the /usr/local blah blah blah with the actual path which you can find by going to usr/local/mysql-9.3 or whatever version and copying the Bin file’s pathname

Then use the command “source .zshrc” to reload the new path
Use “mysql -u root -p” to set up mysql

You can also download mysql workbench as a GUI

Lightning symbol is the button to run the query 

