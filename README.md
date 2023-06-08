# php-test

https://github.com/microsoft/vscode-remote-try-php#things-to-try
Things to try
Once you have this sample opened, you'll be able to work with it like you would locally.

Some things to try:

Edit:

Open index.php
Try adding some code and check out the language features.
Make a spelling mistake and notice it is detected. The Code Spell Checker extension was automatically installed because it is referenced in .devcontainer/devcontainer.json.
Also notice that utilities like Xdebug and the PHP Intelephense extension are installed. Tools are installed in the mcr.microsoft.com/devcontainers/php image and Dev Container settings and metadata are automatically picked up from image labels.
Terminal: Press ctrl+shift+` and type uname and other Linux commands from the terminal window.

Run and Debug:

Open index.php
Add a breakpoint (e.g. on line 4).
Press F5 to launch the app in the container.
Once the breakpoint is hit, try hovering over variables, examining locals, and more.
Running a server:
php -S 0.0.0.0:8080

From the terminal, run php -S 0.0.0.0:8000
Click "Open in Browser" in the notification that appears to access the web app on this new port.
You can view an organized table of your forwarded ports in the 'Ports' view, which can be accessed with the command Ports: Focus on Ports View.
Notice port 8000 in the 'Ports' view is labeled "Hello Remote World." In devcontainer.json, you can set "portsAttributes", such as a label for your forwarded ports and the action to be taken when the port is autoforwarded.
Look back at the terminal, and you should see the output from your site navigations.
Edit the text on line 21 in index.php and refresh the page to see the changes immediately take effect.
Attach debugger to the server:

Follow the previous steps to start up a PHP server and open a browser on port 8000
Press F1 and select the View: Show Debug command.
Pick "Listen for XDebug" from the dropdown.
Press F5 to attach the debugger.
Add a breakpoint to index.php if you haven't already.
Reload your browser window.
Once the breakpoint is hit, try hovering over variables, examining locals, and more.
Install Node.js using a Dev Container Feature:

Press F1 and select the Dev Containers: Configure Container Features... or Codespaces: Configure Container Features... command.
Type "node" in the text box at the top.
Check the check box next to "Node.js (via nvm) and yarn" (published by devcontainers)
Click OK
Press F1 and select the Dev Containers: Rebuild Container or Codespaces: Rebuild Container command so the modifications are picked up.
