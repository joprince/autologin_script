# autologin
Python script to automate login to captive portals.

## Steps
1. Requirments python3, firefox and selenium.
2. Update the path provided in the code to geckodriver.
3. Inspect the login page and update the code [I've used name tags. You can use id or class chage the code accordingly].
4. Thats it. Run the script. 

If you want you can convert this to one click executable file.

If you are using a LINUX system, then add a custom shortcut. Goto add keyboard shortcut. Use the command 
**gnome-terminal -e "path/to/login.py"**.  
Else you can use crontab to run the script every 30 mins and on startup. Open terminal and execute "crontab -e" .
Paste the following command in the file, save and exit.  
*/30 * * * * export DISPLAY=:0; gnome-terminal -- "/path/to/login.py"; exit;  
@reboot export DISPLAY=:0; gnome-terminal -- "/path/to/login.py"; exit;


