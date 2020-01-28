# chumbucket
Does the mindless task of handling Chummer (A Shadowrun 5e Tabletop Character Manager) data synchronizations to AWS S3.

The whole point of this is to allow me the flexibility of running Chummer locally when I am home, and in the cloud when I am traveling.

Because Chummer + RDP to my localbox is *not great*.

Chumbucket will keep as many backup copies of your character if you so desire. A word of caution: Setting HISTORY to 0 in config.ini will result in no sync backup being made. You might lose some data. 

## Installation

1. Clone the Repo or just download the zip from releases. If you clone the repo, be prepared to allow unsigned Powershell scripts. YOU HAVE BEEN WARNED.
2. Put the folder somewhere you will remember later.
3. Make a copy (or rename) config.ini.template to config.ini
4. Edit config.ini to your liking. You can disable syncing of certain things, but at the minimum you need to fill out the AWS API key items.
5. Run chumbucket.ps1 once manually to ensure it finds all your files and uploads them.
6. Repeat the 1-5 on your other system, that currently has NO data available. Check to see that it has pulled down your data.
7. Either set up a scheduled task to repeatedly sync, or put a shortcut in a convenient place to just run it manually.

## Todo
- All of it.