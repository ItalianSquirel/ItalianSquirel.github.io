---
title: "Rough start to Linux..."
published: true
---

Howdy.

Just got a Linux distro up and running im my virtual machine. There were a few hiccups in the process but other than just minor inconveniences it was insanely simple.

First off when I decided to go with linux mint, I liked the look of it and the fact that the interface is close to windows make it an overall easy transfer, so I can go between them just fine. 

The first speed bump on my way to having an amazing desktop environment was the screen resolution in the VM. I logged in and saw that it isn't detecting my monitor nor did it have my screen size in the displays menu in settings and since i didn't want to just scale the screen up (because the qualtiy was trash) i got to work on finding a solution. 

I went to google and looked up adding a custom resolution in linux via the terminal. There were plenty of articles and videos on the matter which is great to see. I got the first result and went to work. 

I typed ```xrandr``` into the terminal to see what my display was named in my case it was Virtual1.

![](https://i.imgur.com/3x493s3.png)

Then I had to calculate the mode line with my monitor's resolution, that was easy I just put [cvt 1920 1080] because my screen resolution was 1920x1080p.

![](https://i.imgur.com/kRKz2kf.png)

Then I copied the mode line (the underlined part) and put it into this command ```sudo xrandr --newmode "1920x1080_60.00"  173.00  1920 2048 2248 2576  1080 1083 1088 1120 -hsync +vsync```. Then after that ran I put in ```sudo xrandr --addmode Virtual1 "1920x1080_60.00"``` with the desired resolution and my display name to add it to the dropdown menu in settings. And last, because I didn't feel like going to settings again just put in ```xrandr --output Virtual1 --mode "1920x1080_60.00"``` to test it before closing the terminal, and bingo, it worked!

one problem was that it wouldn't save so I would have to type that in every time the VM rebooted. TO fix that I just opened terminal and Adding the command to the end of ```~/.profile``` by putting in ```nano ~/.profile``` I added the three commands to the file:

```
sudo xrandr --newmode "1920x1080_60.00"  173.00  1920 2048 2248 2576  1080 1083 1088 1120 -hsync +vsync
sudo xrandr --addmode Virtual1 "1920x1080_60.00"
xrandr --output Virtual1 --mode "1920x1080_60.00"
```
I rebooted.

Welp there was a problem, the commands I was running in the background at startup require a password to run...

I then made it so it didn't need my password to run commands. To do this I  typed ```sudo visudo``` into the terminal. Then add the line ```italian-squirel ALL=(ALL) NOPASSWD: ALL``` BAM! Now it works.

Shortly after figuring th=is whole mess out I actually found that VirtualBox has a digital disk you can put into your VM to fix this issue. I screamed internally. I'm gonna take a break now.

See ya.
