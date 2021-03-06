# EKFiddle v.0.3

A framework based on the Fiddler web debugger to study Exploit Kits, malvertising and malicious traffic in general.

View PPT presentation from BSidesVancouver: https://www.slideshare.net/JeromeSegura/ekfiddle-a-framework-to-study-exploit-kits

# Installation

## Download and install the latest version of Fiddler

http://www.telerik.com/fiddler

Special instructions for Linux and Mac here:

http://www.telerik.com/blogs/fiddler-for-linux-beta-is-here

http://www.telerik.com/blogs/introducing-fiddler-for-os-x-beta-1

## Enable C# scripting (Windows only)

Launch Fiddler, and go to `Tools -> Options`

In the `Scripting` tab, change the default (JScript.NET) to C#. 

## Change default text editor (optional)

In the same `Tools -> Options` menu, click on the `Tools` tab.

* Windows: `notepad.exe` or `notepad++.exe`
* Linux: `gedit`
* Mac: `/Applications/TextEdit.app` or `/Applications/TextWrangler.app`

Close Fiddler

## Download or clone CustomRules.cs into the appropriate folder based on your operating system:

* Windows (7/10) `C:\Users\[username]\Documents\Fiddler2\Scripts\`

* Ubuntu `/home/[username]/Fiddler2/Scripts/`

* Mac `/Users/[username]/Fiddler2/Scripts/`

## Finish up the installation

Start Fiddler to complete the installation of EKFiddle. That's it, you're all set!

# Features

## QuickSave

Dumps current web sessions into a SAZ named (QuickSave-"MM-dd-yyyy-HH-mm-ss".saz) to EKFiddle\Captures\.

## Start VPN

With EKFiddle 0.2, a VPN GUI (.ovpn) is now available inside of Fiddler.
It uses the OpenVPN client on Windows and Linux with ovpn files which you can acquire from commercial VPN providers.
It will open up a new terminal/xterm whenever it connects to a new server, killing the previous to ensure only one TAP adapter is used at any given time. 

* Windows

Download and install OpenVPN in default directory

Place your .ovpn files inside OpenVPN's `config` folder.

* Linux (tested on Ubuntu 16.04)

`sudo apt-get install openvpn`

Place your .ovpn files in /etc/openvpn.

## Import SAZ/PCAP

A shortcut to load SAZ or PCAP captures.

## View/Edit Regexes

View and create your own regular expressions.

## Run Regexes

Run your regular expressions against current web sessions.

## Advanced UI on/off

Toggle between the default column view or extra columns with additional information.

# Uninstalling EKFiddle

Open Fiddler, go to `Tools -> EKFiddle -> Uninstall EKFiddle`

Delete CustomRules.cs
