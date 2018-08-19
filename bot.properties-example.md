# Example of bot.properties with filled values
See the notes below for a detailed explanation of each value.

Notes are also written into the code of the NN-chatbot file.
```
bot.globalUsername=Alisha

bot.site.metastackexchange=https://chat.meta.stackexchange.com
bot.site.stackoverflow=https://chat.stackoverflow.com
bot.site.stackexchange=https://chat.stackexchange.com
bot.site.discord=discord
bot.site.twitch=twitch

bot.homes.stackoverflow=1
bot.homes.metastackexchange=721
bot.homes.stackexchange=1

bot.home.leave=false

bot.stackexchange.admin=1234
bot.stackoverflow.admin=1234
bot.metastackexchange.admin=1234
bot.discord.admin=1234
bot.twitch.admin=MyCreativeTwitchUsername

about.instanceLocation=Bot/UnnamedInstanceTodo

about.creator=Olivia
about.creatorGithub=https://github.com/LunarWatcher
about.github=https://github.com/LunarWatcher/NN-chatbot
about.revision = 1.5.7

bot.trigger=//

bot.nnip=127.0.0.1
```

### Bot's Actual Name
Not the same as the site specific names configured in `creds.properties`.
```
bot.globalUsername=Alisha
```

### Supported Sites
Remove these locally if you want to disable sites.
```
bot.site.metastackexchange=https://chat.meta.stackexchange.com
bot.site.stackoverflow=https://chat.stackoverflow.com
bot.site.stackexchange=https://chat.stackexchange.com
```

Discord and Twitch do not have URLs because their APIs use bot accounts and tokens.
Their names are simply an identifier.
```
bot.site.discord=discord
bot.site.twitch=twitch
```

### Hard-coded home rooms
Hard-coded home rooms cannot be removed through a command.

Discord is not included because it cannot leave specific channels like in the Stack Exchange network.
<!---Why isn't Twitch included?--->
```
bot.homes.stackoverflow=1
bot.homes.metastackexchange=721
bot.homes.stackexchange=1
```

Leave home rooms when the home has been removed.
```
bot.home.leave=false
```

### Hard-coded Admins
Hard-coded admins cannot be removed through command, unlike regular admins who are stored in the database.

Lists of names or IDs are separated by commas.

```
bot.stackexchange.admin=1234
bot.stackoverflow.admin=1234
bot.metastackexchange.admin=1234
bot.discord.admin=1234
bot.twitch.admin=MyCreativeTwitchUsername
```

### Instance Location
The instance location is accompanied by a timestamp for the launch. Timestamps prevent confusion if  multiples of one instance are launched at separate times.
```
about.instanceLocation=Bot/UnnamedInstanceTodo
```

### Bot Meta
Bot meta should only be changed if there is a custom implementation. Otherwise, direct any bugs
and pull requests to the main repo.
```
about.creator=Olivia
about.creatorGithub=https://github.com/LunarWatcher
about.github=https://github.com/LunarWatcher/NN-chatbot
```
### Current Version
```
about.revision = 1.5.7
```

### Trigger
The trigger the bot uses
```
bot.trigger=//
```

### Neural Network IP
The IP address where the neural network is located.
* Defaults to localhost
* Changeable per instance using {trigger}ip

```
bot.nnip=127.0.0.1
```
