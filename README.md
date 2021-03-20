# Bot setup guide

## Part 1: Creating the bot account

1. Go to https://discord.com/developers/applications
2. Login to your discord account
3. Click on `New Application`
4. Enter the name of your bot and press create
5. Click on the `Bot` tab on the left menu bar
6. Click on `Add Bot`
7. Scroll down and enable `PRESENCE INTENT` and `SERVER MEMBERS INTENT`, then press `Save Changes`
8. Press `OAuth2` on the left menu bar
9. Check the `bot` checkbox and press `Copy`
10. You can paste this link in your browser and add this bot to any discord server you want. You can use this link again to add the bot into other servers!

## Part 1.5: Getting the bot token

1. Click on the `Bot` tab on the left menu bar
2. Click on `Copy` under `TOKEN`. Remember, never give this token to strangers, as they can gain full access to your bot if they gain access to this token!

## Part 2: Hosting the bot

0. Download/Clone the bot files
1. Navigate to the folder that contains the bot's code in a file explorer
2. Rename all files ending with `.json.example` to `.json`, removing the `.example`, such as renaming `config.json.example` to `config.json`
3. Fill in the token that you got from `part 1.5` into the config.json

   Here is an example:

   ```
   {
      "PREFIX": "!",
      "TOKEN": "ODE4NDY3Mzc0NzE3OTkzMDAx.YEYfJA.j_vM2raH-LOsGDcZGavrBjqk9hk"
   }
   ```

4. Go to https://nodejs.org/en
5. Download and install NodeJs on your computer/server
6. Start a command prompt/terminal
7. Use the `cd` command to navigate to the folder that cointains the bot's code
8. Type `npm install` in the terminal and then press enter
9. Type `node .` in the terminal to run the bot! Press `ctrl + c` to stop the bot.
