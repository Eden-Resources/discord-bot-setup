# Bot setup guide
## Creating the bot account

1. Go to the [discord developer portal](https://discord.com/developers/applications)
2. Login to your discord account
3. Click on `New Application`
4. Enter the name of your bot and press create
5. Click on the `Bot` tab on the left menu bar
6. Click on `Add Bot`
7. Scroll down and enable `PRESENCE INTENT` and `SERVER MEMBERS INTENT`, then press `Save Changes`
8. Press `OAuth2` on the left menu bar
9. Check the `bot` checkbox and press `Copy`
10. You can paste this link in your browser and add this bot to any discord server you want. You can use this link again to add the bot into other servers!

## Setting up the files

1. You should have git pre-installed if you are using mac or linux. If not, download and install git [here](https://git-scm.com/downloads)
2. Go to the github page of this repo and press `⬇Code`, select `HTTPS`, then copy the link
3. Start a terminal
4. Use the `cd` command to navigate to wherever you want the bot files to be placed in
5. Type `git clone [paste in the link here]` (add sudo if you are on linux and it gives you an error)
6. Login to your github account in the terminal
7. Navigate to the folder that contains the bot's code in a file explorer
8. Rename `.env.example` to `.env`

## Configuration

### Getting the bot token

1. Click on the `Bot` tab on the left menu bar
2. Click on `Copy` under `TOKEN`. Remember, never give this token to strangers, as they can gain full access to your bot if they gain access to this token!
3. Fill in the token into the `.env` file

   Here is an example:
   ```
   ...
   TOKEN=ODE4NDY3Mzc0NzE3OTkzMDAx.YEYfJA.j_vM2raH-LOsGDcZGavrBjqk9hk
   ...
   ```


### Getting the client ID

1. Click on the `General Information` tab on the left menu bar
2. Copy the `CLIENT ID`
3. Fill in the ID into `.env`

   Here is an example:
   ```
   ...
   CLIENT_ID=761048219479421520
   ...
   ```

<!---
### Setting up ngrok for request handling
1. Go [here](https://ngrok.com/download) to download ngrok
2. Unzip the zip file that you just downloaded
3. Get your authentication token [here](https://dashboard.ngrok.com/get-started/your-authtoken)
4. Run `./ngrok authtoken [TOKEN]` at the location that you unqipped the file to. Replace `[TOKEN]` with your authentication token
5. Run `./ngrok http [PORT]`. Replace `[PORT]` with the port that you want to use (if you don't know which port to use, use 3000)
6. Copy the link that is displaying in the window. It should look something like `http://3af3b4364d80.ngrok.io` (not the https one)
7. Paste it into the config.json, after the `"REDIRECT"` attribute
8. Also enter the port you used after the `"PORT"` attribute
-->

<!---
### How to set up google APIs
1. Go to [google developers console](https://console.developers.google.com/)
2. Create a new project
3. Press `+ENABLE APIA AND SERVICES`
4. Search for the API(s) that you want to enable and enable them
5. Go to back to the project page
6. Click on `Credentials` on the left menu bar
7. Click `+CREATE CREDENTIALS`
8. Select `Service account`
9. Fill in the details (does not matter) and press `CREATE`
10. Chose the role by hovering over the drop down > Basic > Owner
11. Press `Continue`
12. Press `Done`
13. Now click into the new service account that you created in the Credentials page
14. Click on `Keys`, then `Add Key`, then `Create New Key`
15. Chose `JSON`, and click `Create`
16. Rename the JSON file that you just downloaded to `client-secret.json` and place it inside your bot's foler

### How to get the service account's adress
1. Open the JSON file that you just downloaded
2. The email is in line 6, like this: `"client_email": "<email>"`

### Additional steps for some APIs
#### Google Sheets
1. Go to your google sheet document in your browser
2. The URL should look something like this: `https://docs.google.com/spreadsheets/d/<DOC-ID>`
3. Copy the ID in the URL and paste it in the `config.json`
4. Return to your google sheet document
5. Press `Share`
6. Share the document to the service account's adress and give it editor perms

#### Google Vision 
1. Enable billing for your project [here](https://cloud.google.com/billing/docs/how-to/modify-project?visit_id=637510599696575187-2745866112&rd=1#enable-billing).
-->

## Hosting the bot
1. Go to the [NodeJs website](https://nodejs.org/en)
2. Download and install NodeJs on your computer/server
3. Start a command prompt/terminal
4. Use the `cd` command to navigate to the folder that cointains the bot's code
5. Type `npm install` in the terminal and then press enter
6. Run `npm install typescript -g`
7. Run `tsc` 
8. Type `node build` in the terminal to run the bot! Press `ctrl + c` to stop the bot.

## Fetching a newer version of the bot
1. Stop the bot using `ctrl + c`
2. Run `git pull`
3. Run `tsc`
4. Run `node build` to start the bot up again
