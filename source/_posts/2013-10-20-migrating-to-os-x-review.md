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

<!-- more -->

Skip to: **[OS X](#os)** ([confusing](#os-confusing), [good](#os-good))

## <a id="os"></a> The Operating System

**OS X Mountain Lion**

The transition from Microsoft Windows to Mac OS X was not as clear-cut advantageous as the [transition from Dell to Apple hardware](/blog/2013/10/18/migrating-to-macbook-review) was. There are some quite strange things for a Windows user to get used to in OS X...



### <a id="os-confusing"></a> Confusing things in OS X (for a Windows user)

**Closing a Window hardly ever ends a program.** Conversely, in Windows, you usually expect that closing a program's main window will end the program. If not, you can always look in the system tray (in fact, the '[notification area](http://en.wikipedia.org/wiki/Taskbar#Taskbar_elements)') to verify whether the program is really dead or not. In OS X, only certain programs seem to die when you close all their windows. This upset me for about an hour when I realised. However, a simple `⌥⇥` (`Option+Tab`) shows all running applications. You can then quit the programs with a simple `⌘Q` (`Command+Q`).

**Full-Screen Apps Only Use One Monitor** This is a very weird decision on the part of Apple. Making an app full-screen will blank out all the other monitors, rendering them useless. However, this will be [fixed in the upcoming OS X Mavericks](http://www.apple.com/uk/osx/preview/#multiple-displays) release. (Note: link will eventually break.)

**Maximising windows is inconsistent in OS X.** Depending on the program, clicking the green + icon in the top left of a window can variously make the window full-height, full-width and full-height, do nothing at all, or go full-height and some arbitrary width. This seems odd for an otherwise highly consistent user interface.

**There is no built-in window snapping in OS X.** One of [my favourite features in Windows](http://windows.microsoft.com/en-GB/windows7/products/features/snap) has been the ability to drag a window to the top, left, or right of the monitor, and have that window either maximise, or snap to the left or right and resize to half the available width. This kind of feature is sadly missing from OS X Mountain Lion. However, there is a brilliant free app called [Better Touch Tool](http://blog.boastr.net/downloads-secondbar-bettertouchtool-2/) which adds window snapping, plus loads of other useful features to window management in OS X.



### <a id="os-good"></a> Brilliant features in OS X

**Mission Control, Exposé, and Spaces, are amazing.** Nuf' said. But really, these three core navigation features are really central to any multi-window workflow on OS X. And, they're pretty much a game-changer, coming from Windows. You can swipe four fingers left or right, to access [as many desktops, 'Spaces,'](http://mattgemmell.com/2011/07/27/using-spaces-on-os-x-lion/) as you need. This is an astonishingly useful feature, especially when you don't have an external monitor. The quickness of a four-finger-swipe-up, to see all open windows and desktops, known as [Mission Control](http://en.wikipedia.org/wiki/Mission_Control_(OS_X\)), is also hugely useful. There is also an under-used four-finger-swipe-down gesture to [show all windows belonging to the current application, 'App Exposé'](http://www.apple.com/uk/osx/what-is/gestures.html#gallery-gestures-expose). I am no longer horrified by the idea of working without [multiple](http://www.codinghorror.com/blog/2004/06/multiple-monitors-and-productivity.html) [external](http://www.codinghorror.com/blog/2010/04/three-monitors-for-every-user.html) [monitors](http://www.codinghorror.com/blog/2008/03/does-more-than-one-monitor-improve-productivity.html).

**[Terminal](http://www.apple.com/osx/apps/all.html#terminal), the command-line of OS X** is a huge breath of fresh air coming from the [neglected Windows command line](http://stackoverflow.com/questions/473839/help-me-make-my-windows-cmd-exe-console-work-more-like-a-linux-terminal). For a start, it provides sane, line-aware text selection, allowing you to select text in the same order as it was printed to the output stream. This is unlike the Windows command line's bizarre treatment of text as a _table_ of characters to be selected in a grid. It also has tabs, so you can easily have multiple sessions open at once in the same window.