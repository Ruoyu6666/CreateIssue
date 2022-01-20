## Install Node.js

1. Download node.js [Windows Binary (.zip)](https://nodejs.org/en/download/) and extract it to desired location
2. Add path of the nodejs folder to the Path environment variable
 - Shortcut Windows key+R and enter `rundll32 sysdm.cpl,EditEnvironmentVariables`
 - Edit Path environment variable: Copy the path where `node.exe` locates and add to environment variable of Path
 
![image](https://user-images.githubusercontent.com/74153282/150339732-dec20e47-6171-4c3e-8ee5-84dced97ee84.png)
 
 ![image](https://user-images.githubusercontent.com/74153282/150340176-bddbc450-caf3-4313-9c64-3a75b6a681e7.png)

3. Open a new command window (Win+R) and type cmd. Type node -v and npm -v to verify the installation. 

## InstallvgithubCsvTools

4. Since there can be error casused by firewall during installing, type `npm config set strict-ssl false` in command line
5. Type 'npm install -g github-csv-tools' in command line to install github-csv-tools
