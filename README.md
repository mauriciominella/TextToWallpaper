# TextToWallpaper
Here is the link to the original scripts: https://askubuntu.com/questions/556723/make-a-text-file-my-automatically-updated-background/556769#556769
Python script which listens to a text file and writes its content to the wallpaper
The script below watches a textfile that you can edit. If the file is changed, it will create a new layer over your wallpaper with the text of the file.

## Options

you can define:

- text size
- text color
- number of columns
- (max) number of lines per column
- border width (around the text blocks)

## How to use

The script uses Imagemagick, you might have to install it first:

```
sudo apt-get install imagemagick
```

Then:

Copy the script below into an empty file and save it as walltext.py.
Edit, if you want specific settings, the options in the head section of the script.
Into the same folder, copy the wallpaper of your choice , name it (exactly) original.jpg

N.B.- It is important that the proportions of your wallpaper match the proportions of your screen's resolution, else the text will not be positioned properly.
In the same folder, create an empty textfile named (exactly) notes.txt. This is the file to make your todolist or whatever you'd like to have on your screen.
Run the script by the command:

```
python3 /path/to/walltext.py
```

Now start editing your text file. Every five seconds, the wallpaper is updated if needed (after you saved the changes)


