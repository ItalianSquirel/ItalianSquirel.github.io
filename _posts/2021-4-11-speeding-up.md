---
title: Speeding Up Windows
published: true
---
---

Howdy.

Just a small thing here today, I just watched a video from **Chris Titus Tech** about speeding up windows by getting rid of most of the bloatware, and since my laptop can always be fatser(and who usies cortana anyway) I decided to do it.

First things first, this script is open source you that means you can mess around with it and make it your own! I will add the youtube video and the respective github link to this repository at the bottom of the post.

---
The script does a lot to make your windows more lightweight such as:

* Removing all Windows Store Apps **EXCEPT** for MS Office, Xbox, and WSL
* Removing Telemetry
* Disabling Cortana
* Deleting variousall kinds of schedules and tasks that rebloat the system
* Removes Other Bloatware (Candy Crush, etc.)
* Fixes problems that other scripts causes (lock screen and personalization options restricted).

---

Without any further ado, Lets get started. To start I opened Power shell as Admin and ran: `iex ((New-Object System.Net.WebClient).DownloadString('https://git.io/JJ8R4'))`.
<br/>
<br/>
<br/>
You should now see a window that looks like this:
![](https://github.com/ItalianSquirel/ItalianSquirel.github.io/raw/master/assets/bloat.JPG)
<br/>
<br/>

Feel free to do what you want with this software but when I used it I only pressed these buttons:
![](https://github.com/ItalianSquirel/ItalianSquirel.github.io/raw/master/assets/image_6483441.JPG)
<br/>
<br/>

I didn't install anynew programs because I already had most of the applications listed including Chocolatey (You should get it!).

After doing these steps my resting CPU Usage went down quite a bit, sadly I didnt record what percentage CPU my laptop was running at but I can tell you that it uis running quit a bit better, I suggest you give this a try if you feel like your pc is a little sluggish or if you just want to get rid of all that bloatware.

Thats all folks!

---
Links:

* [Youtube Video](https://www.youtube.com/watch?v=V27McA7ch6w&t=377s)
* [Chris Titus Tech's website Guide](https://christitus.com/windows-10-optimization-guide/#optimizing-windows-10-settings)
* [The GitHub Repo](https://github.com/ChrisTitusTech/win10script)
* [Chocolatey (Cause why not)](https://chocolatey.org/)