## Install Node.js

1. Download node.js [Windows Binary (.zip)](https://nodejs.org/en/download/) and extract it to desired location
2. Add path of the nodejs folder to the PATH environment variable
 
3. Open a new command window (Windows key+R and type cmd)

![image](https://user-images.githubusercontent.com/74153282/150338937-eab93d56-acba-48c9-8006-e39f31ca2acb.png)


4. Check out the `notifications-starter` branch, then run the following commands in the project folder:


## Talk Code-Along Instructions

If you are here for a code-along portion at a talk, welcome! I'll go over these instructions in the talk, but in case you miss something or are watching from home, here are the steps for coding along.

1. Fork this repo and clone it locally.

2. Check out the `notifications-starter` branch, then run the following commands in the project folder:

`npm install`

`touch .env`

This repository has two dependencies -- `dotenv` and `node-fetch`. `Dotenv` is for protecting your GitHub token and `node-fetch` is for making API calls. Feel free to use `axios`, another package, or `Node` to make the calls if you prefer.

4. Make sure to add `.env` to your `.gitginore` if you plan to push this code to GitHub.

5. Once your GitHub access token is generated, save it to your `.env` file as

`TOKEN=<TOKEN HERE>`

6. Code in `GetNotifications.js` using the comment prompts to write a script that gets your notifications for a repository, saves any of the type `security-alert` to a file, then marks those notifications as read.

## Scripts

Run the following scripts from the `master` branch in the root project directory.

### Create Issues from JSON 

File: CreateIssueFromJSON.js

`cd CreateIssuesFromJSON
node CreateIssuesFromJSON.js`
