# Example of creds.properties with filled values
See the notes below for a detailed explanation of each value.

Notes are also written into the code of the NN-chatbot file.

```
# Stack Overflow
stackoverflow.user.name=Alisha
stackoverflow.user.email=example@example.com
stackoverflow.user.password=1234
stackoverflow.user.id=0123
# Meta Stack Exchange
metastackexchange.user.name=Alisha
metastackexchange.user.email=example@example.com
metastackexchange.user.password=1234
metastackexchange.user.id=4567
# Stack Exchange
stackexchange.user.name=Alisha
stackexchange.user.email=example@example.com
stackexchange.user.password=1234
stackexchange.user.id=8910

# Discord
discord.user.name=Alisha#1234
discord.user.email=token_here
discord.user.password=none
discord.user.id=1234

#Twitch
twitch.user.name=MyCreativeBotUsernameHere
twitch.user.email=Client ID
twitch.user.password=Secret
twitch.user.id=none
twitch.oauth.credential=none

* Add any other sites' password config here
```

## Stack Exchange (SE) Network
Stack Overflow, Stack Exchange and Meta Stack Exchange: The username, email, password and ID for each component of the SE Network.
```
# Stack Overflow
stackoverflow.user.name=Alisha
stackoverflow.user.email=example@example.com
stackoverflow.user.password=1234
stackoverflow.user.id=0123
# Meta Stack Exchange
metastackexchange.user.name=Alisha
metastackexchange.user.email=example@example.com
metastackexchange.user.password=1234
metastackexchange.user.id=4567
# Stack Exchange
stackexchange.user.name=Alisha
stackexchange.user.email=example@example.com
stackexchange.user.password=1234
stackexchange.user.id=8910
```

## Discord
#### Discord Bot Username
The username given to the bot on its Discord account.
```
discord.user.name=Alisha#1234
```

#### Discord Token
The token assigned to the bot when it was registered as an application on Discord.
Register the bot as a Discord Application [here](https://discordapp.com/developers/applications/me).
```
discord.user.email=token_here
```

#### Discord Password
Leave the password value alone; it exists because the system runs on a static implementation, but it's not used
 since Discord bot accounts use tokens instead of the traditional email and password.
 ```
discord.user.password=none
```

#### Discord Bot ID
The bot's user ID associated with the bot account.
```
discord.user.id=1234
```

## Twitch
#### Twitch Username
The username given to the bot on its Discord account.
```
twitch.user.name=MyCreativeBotUsernameHere
```

#### Twitch Client ID
The Client ID assigned to the bot when it was registered as an application on Twitch.

Register the bot as an application [here](https://glass.twitch.tv/console/apps/create).
```
twitch.user.email=Client ID
```

#### Twitch Password
The password for the account associated with the bot.
```
twitch.user.password=Secret
```

#### Twitch User ID
The user ID doesn't matter on twitch; usernames are unique. Leave the value alone.
```
twitch.user.id=none
```

#### Twitch OAuth Key
Get one [here](https://twitchapps.com/tmi/).
Must be logged in as the user who is posting the chat messages
```
twitch.oauth.credential=none
```
