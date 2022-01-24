## Install Node.js

1. Download node.js [Windows Binary (.zip)](https://nodejs.org/en/download/) and extract it to desired location

2. Add path of the nodejs folder to the Path environment variable as follow:
  - Shortcut Win+R and enter `rundll32 sysdm.cpl,EditEnvironmentVariables`
  - Edit Path environment variable: Copy the path where `node.exe` locates and add to environment variable of Path
 
![tempsnip](https://user-images.githubusercontent.com/74153282/150343343-2e7e830a-ebea-4f78-9275-cfc743fc2da7.png)
 
![tempsnip2](https://user-images.githubusercontent.com/74153282/150344410-b7f051fe-d423-489e-a61d-1e0ca9f3e87b.png)

3. Open a new command window (Win+R and enter `cmd`). Enter `node -v` and `npm -v` in command line to verify the installation. 

## Install githubCsvTools

4. Enter `npm config set strict-ssl false` in command line to avoid error casused by firewall during installing package. 

5. Enter `npm install -g github-csv-tools` in command line to install github-csv-tools

## Generate a new token in GitHub

6. Go to setting and generate a oken in Github. Check the box next to “repo” to select all options to allow edit of repositories. Copy the generated token.

## Create a Dataset of Issues

7. Use `CreateIssue.xlsm` and fill out (market) title, body, assignee, milestone and labels. Copy the generated content in Column G and paste it to an empty text file and save it to test.txt. **NOTE** make sure there's no empty line (especially at the end) in the text file.

8. Enter `githubCsvTools test.txt` in command line, replacing `test.txt` with the path of the targeted file in real use. Then enter token, user/organization and repository as requested.

  A sample file.csv and a sample text.txt are given in this repository for testing.
