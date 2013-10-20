---
layout: post
title: "Migrating to OS X&mdash;Review"
date: 2013-10-20 18:00
comments: true
categories:
- OS X
- review
- Apple
- Migrating from Windows to Mac
published: true
---

_This [Mac OS X 10.8 Mountain Lion review]() is part 2 of a [series on migrating from Windows to Mac](/blog/series#migrating-from-windows-to-mac)._ 

> About 6 months ago I (a .NET developer) took over maintenance of an iOS app. This meant I needed to use a Mac, for the first time in 20 years. In order to avoid maintaining 2 separate workstations, I also switched to using OS X as my primary operating system, with Windows in a VM to continue my .NET work. Here's my take on making the switch...

The transition from Microsoft Windows 8 to Mac OS X was not as clear-cut advantageous as the [transition from Dell to Apple hardware](/blog/2013/10/18/migrating-to-macbook-review) was. There are some quite strange things for a Windows user to get used to in OS X. However, 6 months into this experiment, and I really don't think I'll ever go back to a pure Windows environment.

<!-- more -->

Skip to:<br />
**[The Confusion](#os-x-confusion)**
 ([quitting](#os-x-quitting)
| [fullscreen](#os-x-fullscreen)
| [maximising](#os-x-maximising)
| [snapping](#os-x-snapping)) <br />
**[The Good](#os-x-good)**
 ([Mission Control, Exposé and Spaces](#os-x-navigation)
| [Terminal](#os-x-terminal) <br />
**[The Conclusion](#os-x-conclusion)**

## <i class="icon-apple"></i> <a id="os-x"></a> The Operating System

**Mac OS X (10.8) Mountain Lion**

[OS X Mountain Lion]((http://en.wikipedia.org/wiki/OS_X_Mountain_Lion)) is the first Mac OS I've ever used in a work context, and the only one I've used as an adult. Prior to this my only real experience of using a Mac was at school, as an 8 or 9 year old, putting together school newspapers using on [System 7](http://en.wikipedia.org/wiki/System_7) machines. An experience I barely remember now.




## <i class="icon-question-sign"></i> <a id="os-x-confusion"></a> Confusing things in OS X (for a Windows user)

I almost called this section 'The Bad,' but most of the criticisms aren't really issues with OS X _per se._ They're more to do with having 20 years of Windows usage engrained into my psyche. So, here is a treatment of my initial frustrations transitioning to OS X. I've highlighted a few key points that might be useful things to remember for anyone else undertaking the same journey. 



### <i class="icon-remove-circle"></i> Closing a Window in OS X hardly ever terminates a program

Conversely, in Windows, you usually expect that closing a program's main window will end the program's main [process](http://en.wikipedia.org/wiki/Process_(computing\)). If not, you can always look in the system tray (in fact, the '[notification area](http://en.wikipedia.org/wiki/Taskbar#Taskbar_elements)') to verify whether the program is really dead or not. In OS X, only certain programs seem to die when you close all their windows. This upset me for about an hour when I realised I had tens of applications running that I thought I'd stopped. However, a simple `⌥⇥` (`Option+Tab`) shows all running applications. You can then _quit_ each one using a simple `⌘Q` (`Command+Q`). Terminating an application in OS X is always known as 'quitting' an application. To _quit_ is to end a process. You can _close_ windows, but you can only _quit_ applications.

> Note: In OS X, terminating an application is _always_ known as _quitting_ that application. The same terminology applies to processes in general. To _quit_ is to end the process entirely.



### <i class="icon-resize-full"></i> Full-Screen Apps Only Use One Monitor

This is a very weird decision on the part of Apple. Making an app full-screen will blank out all the other monitors, rendering them useless. In my usual three-monitor setup, this renders the 'full-screen' option totally useless. This issue will be [fixed in the upcoming OS X Mavericks](http://www.apple.com/uk/osx/preview/#multiple-displays) release. (Note: that link will eventually break.)



### <i class="icon-plus"></i> Maximising Windows Is Inconsistent

Depending on the program, clicking the green + icon in the top left of a window can variously make the window full-height, full-width and full-height, do nothing at all, or go full-height and some arbitrary width. This seems odd for an otherwise highly consistent user interface.



### <i class="icon-puzzle-piece"></i> There is no built-in window snapping in OS X

One of [my favourite features in Windows](http://windows.microsoft.com/en-GB/windows7/products/features/snap) has been the ability to drag a window to the top, left, or right of the monitor, and have that window either maximise, or snap to the left or right and resize to half the available width. This kind of feature is sadly missing from OS X Mountain Lion. However, there is a brilliant free app called [Better Touch Tool](http://blog.boastr.net/downloads-secondbar-bettertouchtool-2/) which adds window snapping, plus loads of other useful features to window management in OS X.






## <i class="icon-check-sign"></i> <a id="os-x-good"></a> Brilliant Features In OS X

Along with the strange, there are some incredibly well-designed features in OS X, some of which are so good, in fact, that they have permanently altered some of my workflows, and changed my fundamental expectations of an OS.



### Mission Control, Exposé, and Spaces Are Amazing

Nuf' said. But really, these three core navigation features are really central to any multi-window workflow on OS X. And, they're pretty much a game-changer, coming from Windows. You can swipe four fingers left or right, to access [as many desktops (sometimes called 'Spaces')](http://mattgemmell.com/2011/07/27/using-spaces-on-os-x-lion/) as you need. This is an astonishingly useful feature, especially when you don't have an external monitor. The quickness of a four-finger-swipe-up, to see all open windows and desktops, known as [Mission Control](http://en.wikipedia.org/wiki/Mission_Control_(OS_X\)), is also hugely useful. There is also an under-used four-finger-swipe-down gesture to [show all windows belonging to the current application](http://www.apple.com/uk/osx/what-is/gestures.html#gallery-gestures-expose), known as 'App Exposé'.

I am no longer horrified by the idea of working without [multiple](http://www.codinghorror.com/blog/2004/06/multiple-monitors-and-productivity.html) [external](http://www.codinghorror.com/blog/2010/04/three-monitors-for-every-user.html) [monitors](http://www.codinghorror.com/blog/2008/03/does-more-than-one-monitor-improve-productivity.html).



### Terminal, the command-line of OS X

[Terminal](http://www.apple.com/osx/apps/all.html#terminal) is a huge breath of fresh air coming from the [neglected Windows command line](http://stackoverflow.com/questions/473839/help-me-make-my-windows-cmd-exe-console-work-more-like-a-linux-terminal). For a start, it provides sane, line-aware text selection, allowing you to select text in the same order as it was printed to the output stream. This is unlike the Windows command line's bizarre treatment of text as a _table_ of characters to be selected in a grid. It also has tabs, so you can easily have multiple sessions open at once in the same window.




## <a id="os-x-conclusion"></a> The Conclusion

