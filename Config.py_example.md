<!-- Lacking notes for the moment-->

```
import configparser

ownerName = "Olivia" # Required
ownerIds =  { "stackexchange.com": [],
              "stackoverflow.com": [],
              "meta.stackexchange.com": [],
              "discord" : []}  # you can add multiple owners

botName = "Alisha" # Required
ghRepo = "https://github.com/LunarWatcher/NN-chatbot"

trigger = "//"
netTrigger = "@" + botName

config = configparser.ConfigParser()
config.read("private.ini")
CONFIG_KEY = "creds"

email = str(config[CONFIG_KEY]["seEmail"])
sePassword = str(config[CONFIG_KEY]["sePassword"])
discordToken = str(config[CONFIG_KEY]["discordToken"])

homes = {
    "stackoverflow.com": [1],
    "stackexchange.com": [1],# 36
    "meta.stackexchange.com": [721]
}
storageDir = "botStorage/"
startQuiet = True
leaveQuiet = True

enabledSites = {
    "stackoverflow.com" : True,
    "stackexchange.com" : True,
    "meta.stackexchange.com" : True,
    "discord" : True
}

def isSiteEnabled(site: str):
    try:
        return enabledSites[site]
    except KeyError:
        print("Site not found in enabledSites. False is returned when this happens")
        return False

def isAnyEnabled(sites: []):
    for site in sites:
        if(isSiteEnabled(site)):
            return True
    return False
```
