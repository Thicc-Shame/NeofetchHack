# NeofetchHack
A script that I alias neofetch to

It requires a directory (mine is in ~/Documents/Art/Neofetches, change to where you keep yours) of images of the form
waifu_nameX.extension where waifu_name is the name of the waifu in the picture, X is a number (any single character actually, I don't use the number yet), and extension is png or jpg.

Using this script also requires some changes to your neofetch config. I have mine use w3m for the image backend. I have added some fields to the info printed, which the script edits by use of sed.

When run, the script picks a random waifu from the directory, and sets her image as the image in neofetch, and her name (from the filename) in the "waifu" field in the output. The script then runs neofetch.

The script also supports a "--waifu" flag where you can specify a waifu by regular expression, and the script will pick randomly from the matches.
