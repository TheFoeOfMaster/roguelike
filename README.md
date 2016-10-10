#roguelike教程一图形
我最近打算开发一款带有roguelike元素的游戏。我本人并没有深入的玩过任何一款roguelike游戏，只是接触过《伊洛纳》与国产游戏《符石守护者》。在我看来roguelike的特征是地形与装备的随机，人物永久死亡。我所谓的roguelike元素指的就这个。一个毫无rogulike游戏经验的编程爱好者从头开发一款roguelike游戏，其难度可想而知。诚然，网络上存在大量的开源roguelike游戏，其中不乏非常著名的，非常有影响力的作品。我试图阅读tome4的源码，希望能从tome4源码中汲取经验。但这并不是了解roguelike游戏的最好方式。我偶然在roguebasin中发现了一个系列教程。这个教程用Python和libtcod一步一步的开发了一款简单的roguelike游戏。鉴于roguelike游戏中文资料非常少，我希望把这个系列译成中文，方便其他roguelike爱好者参考。（这个教程中的puthon版本好像比较老，加上本人英文不是很好，阅者见谅）
##设置
OK,既然我们下定决心开发一款roguelike游戏，那让我们开始吧！

If you haven't yet, download and install Python 2.7. Any version of Python 2, from 2.6 and above should be fine, but the latest update (of Python 2, not Python 3) is of course always preferable. There are reports that for older versions of libtcod on 64-bit Windows (Windows 7) that the 32 bit version is preferable, since the 64 bit version of Python seems to cause problems with libtcod. This was been tested on Windows 10 with libtcod 1.6, and was not reproducible, so it's up to you. It's probably advisable to go with 32 bit just to keep things simple, and when you're gone through the tutorial look at switching to 64 bit if it matters to you to do so, and if you do encounter errors specifically related to this, report them on the libtcod bug tracker.
Download the latest release of libtcod 1.6 and extract it somewhere. Be warned that both Python and libtcod must either be both 32 bit, or both 64 bit. If you get dll loading errors, getting this wrong is the most likely cause.
Now to create your project's folder. Create an empty file with a name of your choice, like firstrl.py. The easiest way to use libtcod is to copy the following files to your project's folder:
The libtcodpy directory from the python sub-directory.
libtcod.dll on Windows, probably libtcod.so on Linux
SDL2.dll on Windows, something else on Linux
A font from the fonts folder. We chose arial10x10.png.



