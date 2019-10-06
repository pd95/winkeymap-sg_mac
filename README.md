# "Swiss German" Mac Keyboard Layout for Developers

## The problem

If you are a developer working normally on a Mac keyboard, you know the problems, when you have to do your work on a keyboard with PC layout:
Suddenly you are missing keys like `@[]{}\|`

Even worse: If you try to connect the Mac keyboard to a Windows PC you suddenly see the keys `<` and `§` are swapped!?


## The solution

I had exactly above issue: I've added a PC to my computer setup and wanted to use the Apple Magic Keyboard with all my computers. After installing Windows on my PC, I had the impression that it was nearly unusable (mainly because I didn't know the SG PC layout by hard and because two keys were swapped).
After a long web search I've come to the conclusion that there was no such thing ready to download... but Microsoft provided a tool called **Microsoft Kayboard Layout Creator** [(available here)](https://www.microsoft.com/en-us/download/details.aspx?id=22339) which can be installed on Windows 10 after resolving .NET framework dependencies [(see here)](https://answers.microsoft.com/en-us/windows/forum/windows_10-hardware/microsoft-keyboard-layout-creator-14-instalation/092881f1-470b-4a66-889f-59e868c6b25a).

It's a rather good tool, but I had to realize that Windows does not support the `alt` and `alt + shift` combinations. This is why I used `altgr` (=`ctrl + alt`) and `altgr + shift` as replacement four our beloved combinations.
This setup helped me to create the `SG-Mac.klc` and `SG-Mac_S.klc` keyboard mappings. You can install above tool yourself, and use the `*.klc` files to produce the binaries I've published under [releases](https://github.com/pd95/winkeymap-sg_mac/releases/).

The `SG-Mac_S` mapping (`*.klc` and corresponding binary `sg-mac_s.zip`) has the `<` and `§` keys swapped. This version should be used if you connected an Apple Keyboard to Windows. 

The `SG-Mac` mapping (`*.klc` and corresponding binary `sg-mac.zip`) has no swapped keys. This version should be used if you have a standard PC keyboard (e.g. from Logitech) connected but you want to use the "muscle memory" from Mac OS. 
Please note: *it has not yet been tested by myself, as I do not have a corresponding keyboard available.*


## The conclusion

With the keyboard mappings provided here, it is possible to find the relevant keys, but nevertheless our brain has to adjust. Instead of pressing `alt + shift + 7` for a `\` key, you will have to press `ctrl + alt + shift + 7` (= one key more), or if your keyboard has `altgr` (right beside the spacebar), you can use `altgr + shift + 7`.


## Installation

Download from the [latest release](https://github.com/pd95/winkeymap-sg_mac/releases/) page the desired binary, extract it's content and run the `setup.exe`. This will install the appropriate version for your system. 

If you are not happy with it, you can uninstall it from the "Apps & Features" section in your Windows Settings. The app is called `Swiss German - Mac Layout for Developers`. 
Even better, if you have ideas for improvements, please contact [me](mailto:pd95@users.noreply.github.com).
