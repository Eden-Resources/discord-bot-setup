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

1. [Clone this GitHub Repo](https://eden-resources.github.io/how-to-git-clone/)
2. Navigate to the folder that contains the bot's code in a file explorer
3. Rename all files ending with `.json.example` to `.json`, removing the `.example`, such as renaming `config.json.example` to `config.json`

## Getting the bot token

1. Click on the `Bot` tab on the left menu bar
2. Click on `Copy` under `TOKEN`. Remember, never give this token to strangers, as they can gain full access to your bot if they gain access to this token!
3. Fill in the token into config.json

   Here is an example:
   ```
   ...
   "TOKEN": "ODE4NDY3Mzc0NzE3OTkzMDAx.YEYfJA.j_vM2raH-LOsGDcZGavrBjqk9hk"
   ...
   ```

## Getting the client ID and secret

1. Click on the `General Information` tab on the left menu bar
2. Copy the `CLIENT ID`
3. Fill in the ID into config.json

   Here is an example:
   ```
   ...
   "ID": "761048219479421520"
   ...
   ```
4. Copy the `CLIENT SECRET`
5. Fill in the secret into config.json

   Here is an example:
   ```
   ...
   "SECRET": "c9sPUBgO1cj4y3v-wK9rNKb5jOVgkiIe"
   ...
   ```

## Hosting the bot

1. Go to the [NodeJs website](https://nodejs.org/en)
2. Download and install NodeJs on your computer/server
3. Start a command prompt/terminal
4. Use the `cd` command to navigate to the folder that cointains the bot's code
5. Type `npm install` in the terminal and then press enter
6. Type `node .` in the terminal to run the bot! Press `ctrl + c` to stop the bot.
