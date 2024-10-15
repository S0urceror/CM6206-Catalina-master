# CM6206
CM6206 Driver for MacOS, works at least at Sequoia without codeless kexts

Updated by S0urceror to continue if it cannot exclusively open the CM6206 interface. It just works anyway. No other changes made to code from Dr.Lex and / or LuisLis

I'm making this since it took me a really long time to find a solution. Before you use this also make sure to try a lot of USB ports since sound worked on some but optical didn't. 

Thanks to: https://www.dr-lex.be/software/cm6206.html

## Compile 
* Open xcode Project and click play button 
* Click show finder for product and get your **cm6206int** file  

## Installation 

If you have Catalina get a tool that can unlock I use [Hackintool](https://github.com/headkaze/Hackintool). 

Click to unlock

![Imgur](https://i.imgur.com/2whO5kc.png)

Input your account password

![Imgur](https://i.imgur.com/zus6Pvr.png)

Run 

0. copy cm6206init file into the git. Then, cd into the location of downloaded package
  
1. ``sudo mkdir /Library/Application\ Support/CM6206``

2. ``sudo ./fixperm.sh``

3. ``sudo cp cm6206init /Library/Application\ Support/CM6206``

4. ``sudo cp Installer/be.dr-lex.cm6206init.plist /Library/LaunchDaemons``

5. Restart 
