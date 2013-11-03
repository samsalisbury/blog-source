---
layout: post
title: "Windows Virtualisation Review"
date: 2013-10-30 21:36
comments: true
categories:
- review
- Apple
- Migrating from Windows to Mac
- Virtualisation
- Windows
published: false
---
_This [Workstation virtualisation review]() is part 3 of a [series on migrating from Windows to Mac](/blog/series#migrating-from-windows-to-mac)._

>I'm a .NET developer, and have recently [made the switch](/blog/2013/10/18/migrating-to-macbook-review) from using Windows--_exclusively, for the past two decades--_[to Mac OS X](/blog/2013/10/20/migrating-to-os-x-review), running Windows in a virtual machine so I can continue to use Visual Studio and IIS for dev work. I hope this review will help you decide which virtualisation app is right for you.

Skip to:
[Oracle VirtualBox](#oracle-virtualbox) |
[VMware Fusion 6](#vmware-fusion) |
[Parallels Desktop 9](#parallels-desktop) |
[Conclusion](#conclusion)




## Why This Review?

The choice of virtualisation environment, it turns out, is a pretty consequential one when you're working in a Windows VM all day. I hadn't expected there to be such big differences between the various options... I hope this review will help you decide which is right for you.

Caveats:

- I run Windows exclusively for Visual Studio and IIS
- I do not use an external mouse or keyboard, only the trackpad and keyboard built-in to the 15&ndash;inch [MPB](http://www.apple.com/uk/macbook-pro/)
- These reviews are based on fresh installs of Windows 8.1 into each product, running on OS X Mavericks on a MacBook Pro (16GB RAM/512GB Flash Storage/Core i7 2.7GHz).




## VMware Fusion 6

### Pros

#### <i class="icon-ok"></i> Good performance
The actual VM performance, once it's running, is good, almost like running Windows 8.1 on bare metal. However, resuming a suspended VM is really slow, which is a pain when you want to start and stop often.

#### <i class="icon-ok"></i> Very Stable
I haven't managed to make it crash :)

#### <i class="icon-ok"></i> The Hash symbol `#` can be typed easily
If you close your eyes and imagine the keyboard in front of you is laid out like a normal PC/Windows keyboard, then typing `#` feels natural.

### Cons

#### <i class="icon-remove"></i> No Apple keyboard layout for Windows
If you use an Apple keyboard, like the one built into the MacBook Pro, then you'll presumably want the keys to correspond with what's printed on them. With VMware, you'll have to close your eyes and imagine you have a Windows keyboard in front of you. Pretty confusing.

#### <i class="icon-remove"></i> Edge swipes do not work on Windows
Not everyone likes these edge swipes, used to show the charms bar on Windows. However, if you do want the use these gestures, you won't be able to using VMware Fusion out of the box.

#### <i class="icon-remove"></i> Does not mount virtual hard disks on OS X
Older versions of VMware used to ship with a really useful tool for mounting virtual hard disks as volumes on OS X. This was great when you wanted to access those volumes from, e.g. Terminal on OS X. Sadly, this is no longer an option with VMware, though you can share folders between OS X and the virtual machine.

#### <i class="icon-remove"></i> Nags to install McAffee AntiVirus
When you've paid for software, you don't expect to be nagged.

#### <i class="icon-remove"></i> 'Unity' mode isn't usable
'Unity' is the name VMware gives to the same feature named 'Coherence' in Parallels Desktop, which is the ability to run Windows apps as if they were native Mac Apps, so you can use OS X to manage your Windows windows, and Cmd+Tab through both Windows and Mac apps together. Unity mode is totally broken for Visual Studio in VMware Fusion 6, For example 'Windows+Up' (to maximise) renders the window irrecoverably half off-screen. I haven't tried it with other apps, but it doesn't look promising.

#### <i class="icon-remove"></i> Defaults to unusable resolution on Retina displays
For some reason, when you first set up Windows using VMware, it will chose to 'Use full resolution for Retina display', but it won't tell Windows about the extra-high DPI, rendering fonts far too small to read on a retina screen. Tip: You can fix this by unchecking the option in the machine settings under 'Display'.





## <a id="parallels-desktop"></a> Parallels Desktop 9

### Pros
#### <i class="icon-ok"></i> Great Performance.
The machine feels like it's running on bare metal, suspending and resuming is also really fast, even with 8GB RAM on the VM.

#### <i class="icon-ok"></i> Windows behaves like OS X.
#### <i class="icon-ok"></i> Installs Apple (UK) keyboard layout as standard.
There's an option to flip back to non-Apple keyboard layout if you prefer, but using the Apple keyboard layout with the built-in Apple Keyboard on an MBP make a lot of sense to me.
#### <i class="icon-ok"></i> Works seamlessly with mix of Retina and non-Retina screens
Out of the box, Parallels automatically picks the best settings for working on a Retina display, and if you're on a mix of Retina and non-Retina displays, it just works, seamlessly, to keep everything looking as you would expect.

#### <i class="icon-ok"></i> Coherence mode highly usable
'Coherence' is what Parallels call the same feature as 'Unity' in VMware Fusion. The difference is that in Parallels, this is actually a usable feature, and lets you easily mix and match Mac and Windows apps on screen at the same time. There are a few visual glitches with Visual Studio floating windows, and occasionally Parallels seems to get confused about which window is on top, but on the whole this is a usable integration.

Additionally, in Coherence mode, the Windows notification area (which many call the tray) is displayed alongside your Mac notification area icons (the time, battery meter etc). This means you hardly ever need to switch back to 'windowed' mode, as all of the useful bits of Windows are accessible directly. In Windows 8.1, the newly-restored start button even appears right in your Mac system dock, ready for action.

#### <i class="icon-ok"></i> Mounts virtual hard disks on OS X as standard
This is a really useful feature, meaning that whilst the VM is running, you are able to directly access the virtual hard drives inside Parallels from your Mac. Since OS X has a decent command-line interface, sadly missing from Windows, you can fire up Terminal in OS X, then `cd /Volumes/C` and you have full access to your virtual C drive to do all sorts of things, like use Git or move and copy files, with the full power of a [POSIX compliant](http://en.wikipedia.org/wiki/POSIX) operating system.

#### <i class="icon-ok"></i> Windows keyboard shortcuts work as expected
So, your standard Windows window-mangement shortcuts, e.g. Win+Up to maximise, Win+Left or Right to snap Windows to the left or right behave normally. You can even hit whichever key you've mapped to the Windows key to bring up the start screen, as long as you have a Windows app focussed when you hit it.

### Cons
#### <i class="icon-remove"></i> Coherence mode gets confused with Visual Studio
Visual Studio is a complex beast, and often when using floating windows for things like unit test results, search dialogues etc., the screen redraw doesn't seem to happen when it should, leaving unresponsive ghosts of windows on the screen. This is really annoying, but as long as you keep windows docked, or not on-top of the main Visual Studio window, there seem to be no problems. I really hope Parallels fix this sometime soon.

#### <i class="icon-remove"></i> Possible to lose windows in Mavericks
Occasionally when dragging a window from one monitor to another in Mavericks, the window can end up in an unknowable place. The only way to correct this seems to be by unplugging the external monitor and plugging it back in, at which point the window is usually restored to a sensible location.

#### <i class="icon-remove"></i> Unstable 'Adaptive Hypervisor'
The Adaptice Hypervisor feature causes massive instability, and constant crashes with Mavericks host and Windows 8.1 guest. This might have been fixed in a recent update, but I'm scared to try it again after my initial experience.

#### <i class="icon-remove"></i> Free trial a bit of a pain
The free trial only lasts for 2 weeks, and it nags for license key on every machine launch. Having said that, it blows the competition out of the water, so you're probably best off just paying up and getting it over and done with.




## Conclusion

If you're a Mac user, and you like the way a Mac works, then you'll definitely prefer Parallels Desktop over VMware Fusion. Parallels provides really in-depth integration between your Windows and Mac apps, top-notch performance, and sensible defaults. You still feel like you're using a Mac, but with the convenience of being able to run Windows apps when you need to.

If you're a Windows user, and pretty much reject OS X's design and usability, then you might be more at home using VMware Fusion, since that seems to expect you will be using a non-Apple keyboard, and will never want to run Mac and Windows apps side-by-side. (It presumes you will want to run Windows inside a window, or full-screen.) In this case, though, I would probably recommend looking at [Boot Camp](http://www.apple.com/uk/support/bootcamp/) since this will give you greater performance on Windows.





The very first thing I needed on my new Mac was a Windows environment, to continue my _business-as-usual_ .NET dev work, whilst I picked up Ruby and iOS projects on the side. Since I'm lazy and I hate waiting for computers to reboot, even if it is startlingly fast, BootCamp was simply out of the question for me. _I needed a Windows VM.__ 

The first thing I tried, it being a familiar name to me, was [VMWare Fusion](http://www.vmware.com/uk/products/fusion/). I was disappointed by its integration with OS X for a number of reasons. Its defaults just aren't sensible, at least not for someone just getting used to OS X, and performance (at least back when I tested it) wasn't up to scratch for intense workstation usage. I guess most people want to use their Windows VM like they're using Windows, but I would rather simplify my life by having the same set of key bindings and UI conventions on both my Windows VM and my primary OS. Edit: I hear that Fusion's performance has improved a lot since then.

So, with Fusion out of the picture, I picked up my next most familiar old virtualisation solution... [VirtualBox](https://www.virtualbox.org/), the long-time saviour for front-end developers testing on different verisons of Internet Exeplorer. I used VirtualBox for a day, which, despite reasonable performance and a price that cannot be beaten, just lacked a bit of fluidity in its integration with OS X, and performance wasn't anywhere near where I needed it for hardcore Visual Studio work.

>I would rather simplify my life by having the same set of key bindings and UI conventions on both my Windows VM and my primary OS

The last one on my list, since I hadn't heard of it before, was Parallels Desktop, from Parallels; despite its many imperfections, this one just seems to be close enough to the sweet-spot that it's the one I've continued with