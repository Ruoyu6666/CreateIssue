## Install Node.js

1. Download node.js [Windows Binary (.zip)](https://nodejs.org/en/download/) and extract it to desired location
2. Add path of the nodejs folder to the Path environment variable as follow:
  - Shortcut Windows key+R and enter `rundll32 sysdm.cpl,EditEnvironmentVariables`
  - Edit Path environment variable: Copy the path where `node.exe` locates and add to environment variable of Path
 
![tempsnip](https://user-images.githubusercontent.com/74153282/150343343-2e7e830a-ebea-4f78-9275-cfc743fc2da7.png)
 
![tempsnip2](https://user-images.githubusercontent.com/74153282/150344410-b7f051fe-d423-489e-a61d-1e0ca9f3e87b.png)

3. Open a new command window (Win+R) and type cmd. Enter `node -v` and `npm -v` in command line to verify the installation. 

## InstallvgithubCsvTools

4. Enter `npm config set strict-ssl false` in command line to avoid error casused by firewall during installing package. 
5. Enter `npm install -g github-csv-tools` in command line to install github-csv-tools

## Generate a new token in GitHub

6. Go to setting and generate a oken in Github. Check the box next to “repo” to select all options to allow edit of repositories. Copy the generated token.

## Create a Dataset of Issues

7. Create a CSV and add the column headers with: title, body, assignee, state, milestone, labels. 
   One can use the help of CreateIssue.xlsm. Copy the generated content in Column F and paste it to a empty text file. Then change its extension name to .csv to get the csv file for uploading issues.  
   
8. Enter `githubCsvTools myFile.csv` in command line, replacing “myFile.csv” with the path of the targeted csv file. Then enter token, user or organization and repository as requested

A sample file.csv is given in this repository for testing. 
