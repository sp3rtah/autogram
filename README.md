<p style="text-align: center;">
    <img src="https://raw.githubusercontent.com/sp3rtah/autogram/main/autogram.png" align="middle" alt="Autogram">
<p>

## `0x00 An efficient asyncronous Telegram bot API wrapper!`
Autogram is a telegram BOT API wrapper with focus on simplicity and performance.

## `0x01 Why AutoGram?`
I need a bot framework that makes it easy to administer control remotely.

Autogram has a built-in webhook endpoint written using Bottle. Therefore, if you have a public IP, or can get an external service to comminicate with `localhost` through a service like ngrok (I use it too!), then set that endpoint as AUTOGRAM_ENDPOINT in your environment variable, or inject its value in the bot config during startup, pointing to `lport` defined in configuration file. If the public address provided is not accessible, the program will use polling to fetch updates.
You add functionality to Autogram bot py implementing and adding callback functions. The bot will therefore work with available callbacks, and will continue to work even if none is specified! This allows the bot to work with available features, despite missing user-implemented handlers for specific updates.

## `0x02 Currently implemented update types`
- todo: re-implementing

## `0x03 Upcoming features`
- Add onNotification handlers.
- Plans to cover the entire telegram API.
- Escape special characters internally.

### `footnotes`
- If the `telegram token` is missing in `config file`, or is INVALID, the bot will terminate.
- `Polling` can be implemented by the user, while feeding data to the bot through `bot.parseUpdate(...)`
- Autogram searches for bot `token` in the specified `config file` before resolving to env variable value.
- Don't run multiple bots with the same `TOKEN` as this will cause update problems
- Sending unescaped special characters when using MarkdownV2 will return HTTP400
- Have `fun` with whatever you're building `;)`

## `unlock sublime text 4 license`
This guide also works for linux. The file that needs to be replaced is located in: /opt/sublime_text/sublime_text in case of debian based systems. (Ubuntu, Debian etc.)

Here are the instructions that I followed:

1, Go to https://hexed.it/
2. Click Open File in the top left corner and select /opt/sublime_text/sublime_text
3. Press CTRL + F or on the Search for bar in the left panel and look for: 80 78 05 00 0f 94 C1
4. Now in the editor, click on the first byte (80) and start replacing each byte by: C6 40 05 01 48 85 C9
5. Finally, in the top left corner again, click on Export Button. This will download the file in your Downloads Folder.
6. Execute sudo cp ~/Downloads/sublime_text /opt/sublime_text/sublime_text to replace the original file.
