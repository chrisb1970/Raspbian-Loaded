Raspbian-Loaded
===============

Raspbian Totalally Loaded

Subject: Raspberry Pi Raspian

So as I was researching using the Pi for a project
and trying to get my Pi setup to do the things I wanted it to do.

I realized that I was spending alot of time setting up the Pi.
Making mistakes and redoing the Raspian setup from scratch over and over and over.

I came to the conclusion that wouldn't it be easier if people would just put up a Raspbian Distro
with all the trimmings and just remove what you don't need... 

So Here's what I did... with Raspbian downloded from http://raspberrypi.org

1. Updated to the Latest Distro which is not what is posted (Half Baked and not consitantely kept up) 3.12.22+

2. Set eth0 to static IP (192.168.1.50)

3. Installed TP-Link TL-WN725n Driver (More half Bake information..) Static IP Set to the same Ip as the eth0
so that you can use either on with the same ip (Danger do not use both at the same time creates an IP conflict:: 
I recomend changing the WLAN0 IP if you need to use both that way you will always have a default on the hardwire to access SSH and Webmin)

4. Installed Webmin https://192.168.1.50:10000 (Definitely a cool feature managing your Pi with a GUI and not have to boot into desktop mode which is slow and sluggish and has to have a KVM (Keyboard, Video, and Mouse Connected) )

LAMP (Wierd but I found only one Raspbian LAMPi and it doesn't work. WOW really LOL. So here I go tryin to make things easy for someone else)

5. Installed Apache with ftp access to the Default port 80 website

6. Installed Mysql (I did not configue MySQL I figure that the user would want to for security incase they forget to change U & P)

7. Installed PPP (Perl, PHP, Python)

Logins
pi = Cbbyrd (User) (Desktop, SSH)
root = Cbbyrd (User) (Desktop, Webmin, SSH)
Byrdadmin = Cbbyrd (Website Ftp User) 192.168.1.50

eth0 IP = 192.168.1.50
wlan IP = 192.168.1.50
Website = http://192.168.1.50 on port 80
Webmin = https://192.168.1.50:10000
FTP = ftp://192.168.1.50:21

So the reason I'm doing this is to pay it forward for all of the resources that I used to get my project going.

Since Literally 90% of those resources either didn't work (The author/s probably just forgot that one important detail. I know "How cliche" LOL). or were just straight out wrong or simply just supplied half baked info or maybe they were "Baked" when they posted the info. Now I'm no expert by no means at all but, It would be nice if we could have good learning material and a distro that you dont have to fight with.. Especially when the project isn't trying to learn how to get Pi working. So here is my attemp. 

Just to be clear I am not in anyway shape or form trying to insult anyone or to say I am better than anyone But, can the people who post the articles to help please make sure that they are actully providing helpful info and or code..

For example why post an example that has 50 lines of code when the same thing could be achieved in some cases with 10  lines of code.Isn't it better to light weight and efficient to save memory and resources and if you want to give a more elaborite script please make sure it actully works..

