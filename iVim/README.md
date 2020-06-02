# iVim

iVim is a project that brings the vim editor to the iOS system.

Type `:help ios` in iVim for more detailed information.

## Features

### Font management

Besides some system and embedded monospace fonts, iVim allows users to import and use their own custom fonts.
Also, iVim provides commands for more intuitive and efficient font management.

### Extended keyboard

By introducing compact buttons, iVim covers as many keys as possible in its extended keyboard, so that you can input symbols without switching among key groups. Moreover, you can customize it to meet your own special needs.

### Multistage language input

iVim adds support to multistage input languages such as Chinese or Japanese. 

### Sharing

Through sharing, iVim makes its editing power available to more apps.
Via the share extension, iVim can import text or text files from, or export to other apps.
Via the document picker, you can also import or edit files or directories in iCloud Drive or documents providers, without leaving iVim.

### External hardware keyboard

iVim supports external hardware keyboards well, just connect your favorite one to the device and start typing. If you are using a standard English keyboard, you can remap the `caps lock` key, too.

### Auto restore

After an app termination, iVim restores the last editing session automatically on launch. So you don't have to worry about data losing any more. And you can disable it in Settings.app if you prefer the old way.

## How to install it

### App Store
iVim is now on [App Store](https://itunes.apple.com/us/app/ivim/id1266544660?mt=8)

### Source code
1. Open iVim.xcodeproj in Xcode
2. In General > Identity of target iVim and iVimShare, change their bundle identities to your own unique ones, and select your Apple ID to sign them. As to the App Group, it requires a paid Apple ID. If yours is, change the App Group identifier for these two targets to your own; if not, just turn them off (the only difference is that you cannot share text to iVim when it is off)
3. Connect your device via USB to your computer, and select it as the Destination of iVim
4. Run iVim, Xcode will install it onto your device
5. A free Apple ID may need to do this every 7 days

## Caveats

Normally, you can use iVim as vim on other platforms.
However, there are some points worth mentioning due to iOS system's personality:
1. there is no shell. You cannot call external shell commands.
2. iVim is sandboxed. It means you don't have direct access to files of other apps if not via the sharing feature.

## Giants' shoulders

iVim was inspired by and based on 3 projects:
1. [vim - the official Vim repository](https://github.com/vim/vim)
2. [Vim port from Applidium](https://github.com/applidium/Vim)
3. [VimIOS - A port of Vim to iOS 9+](https://github.com/larki/VimIOS)

Without them, iVim wouldn't begin.

Also, without violating the copyright of Vim, feel free to make modifications to meet your own needs.
