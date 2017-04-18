# A hight quality tools to reverse engineering code from android.
This project aims to select the best tools, to get the code from apk to .java.
A second objective is set the state of art for reverse engineering tools (Apr, 2017).


![](img/1-goal.png)
Lets Go! This project is maintained by @nextco

> No process guarantees 100% code reversion
> but surely we can achieve clues to ensure the highest accuracy.


## The process 
Install, intense test the tools, no short path and select the best.  
Tested on Arch Linux & Windows 8.1 Pro  
Time Spend: 5 days  

## Background
A curated list is create by [Aditya Agrawal](https://github.com/exploitprotocol/mobile-security-wiki)
[The preview](https://mobilesecuritywiki.com/#-reverse-engineering-tools-)


## Get info of Apk
### Goal -  Get AndroidManifest.xml
Get permissions, activity names, package names
- Primary tool: ClassyShark 8.0 [Download](https://github.com/google/android-classyshark/releases) by google
![](img/classyshark-manifest.png)  


ClassyShark is also useful to accurate spy the class, constructors, variables and method names
<p align="center">
  <img src="img/classyshark-spy.png">
</p>

### Goal -  Get Resources
Like a images, assets, html, sounds, js

- Primary tool: Apktool 2.2.2 [Download](https://ibotpeaches.github.io/Apktool/) by ibotpeaches
<p align="center">
  <img src="img/apktool-resources.png">
</p>

## Get .jar from .apk
.dex files need translated to java bytecode, this process are critical because of this output depend the accuracy on obtained code

- Primary tool: enjarify 1.0.3 [Download](https://github.com/Storyyeller/enjarify) by Storyyeller
![](img/enjarify.png)  

I know dex2jar, on this project aim to select the best tools currently, dex2jar is careless and outdated.

## Get .java from .jar
Fortunately on this point are good choices, they are sorted by use.
- Show Java Android App [Download](https://play.google.com/store/apps/details?id=com.njlabs.showjava)
![](img/show-java.png)
![](img/show-java-1.png)

- jadx-gui [Download](https://github.com/skylot/jadx)
![](img/jadx.png)
  

- jd-gui
<p align="center">
  <img src="img/jd-gui.png">
</p>
  

- CFR 0_121 [Download](http://www.benf.org/other/cfr/)
<p align="center">
  <img src="img/cfr.png">
</p>  

- d4j-procyon [Download](https://secureteam.net/d4j)
![](img/d4j.png)

Also tested, FernFlower & Krakatau unsuccessfully

## Extra - Android Player
This is special category, because i want Play Store, Games, Apps a virtual replace of my android on PC, not for dev. A complete replace for phone on pc for daily use.

- Primary tool: Nox Player 3.8.1.1 [Download](https://www.bignox.com/)
<p align="center">
  <img src="img/nox-player.png">
</p>

Also test BlueStacks to lag for me.

## Next Steps.
On next steps for dev app best emulator are of course, Android Emulator
<p align="center">
  <img src="img/android-emulator.png">
</p>