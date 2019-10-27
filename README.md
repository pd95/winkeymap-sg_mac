# "Swiss German" Mac Keyboard Layout for Developers

## The problem

If you are a developer working normally with a Mac keyboard, you know the problem when you have to work on a keyboard with Windows PC layout:
Suddenly you do not find important keys like `@[]{}\|`

Even worse: If you try use the Mac keyboard with the Windows PC, you suddenly see the key `<` and `§` swapped!?

I experienced exactly this issue: I've added a Windows PC to my setup and wanted to use my Apple Magic Keyboard withit. After installing Windows, I had the impression that it was nearly unusable to work with (mainly because I didn't know the Swiss German PC layout by heart and because the two keys `<` and `§` were swapped).


## The solution

After a long web search I've come to the conclusion that there was no such thing to download which solved my problem... but Microsoft provides a tool called **Microsoft Keyboard Layout Creator** [(available here)](https://www.microsoft.com/en-us/download/details.aspx?id=22339) which can be installed on Windows 10 (after resolving .NET framework dependencies [(see here)](https://answers.microsoft.com/en-us/windows/forum/windows_10-hardware/microsoft-keyboard-layout-creator-14-instalation/092881f1-470b-4a66-889f-59e868c6b25a)).

It's a rather good tool, but I had to realise that Windows does not support the `alt` and `alt + shift` combinations, which are used on macOS. This is why I had to use `altgr` (=`ctrl + alt`) and `altgr + shift` as a replacement for our beloved combinations.
This setup helped me to create the `SG-Mac.klc` and `SG-Mac_S.klc` custom Swiss German keyboard mappings for Windows. You can install above tool yourself, and use the `*.klc` files to produce the binaries I've published under [releases](https://github.com/pd95/winkeymap-sg_mac/releases/).

The `SG-Mac_S` mapping (`*.klc` and corresponding binary `sg-mac_s.zip`) has the `<` and `§` keys swapped. This version should be used if you connect an Apple Keyboard to Windows. 

The `SG-Mac` mapping (`*.klc` and corresponding binary `sg-mac.zip`) has no swapped keys. This version should be used if you have a standard PC keyboard (e.g. from Logitech) connected but you want to use the "muscle memory" from trained during your macOS time. 
Please note: *ATM this version has not yet been tested by myself, as I do not have a corresponding keyboard available.*


## The conclusion

With the keyboard mappings provided here, it is possible to find the relevant keys, but nevertheless our brain has to adjust. Instead of pressing `alt + shift + 7` for a `\` key, you will have to press `ctrl + alt + shift + 7` (= one key more), or if your keyboard has `altgr` (right beside the spacebar), you can use `altgr + shift + 7`.


## Installation

Download from the [latest release](https://github.com/pd95/winkeymap-sg_mac/releases/) page the desired binary, extract it's content and run the `setup.exe`. This will install the appropriate version for your system. 

If you are not happy with it, you can uninstall it from the "Apps & Features" section in your Windows Settings. The app is called `Swiss German - Mac Layout for Developers`. 
Even better, if you have ideas for improvements, please contact [me](mailto:pd95@users.noreply.github.com).
