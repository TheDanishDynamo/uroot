# uroot (Uncomplicated Root)

Python wrapper for adb. Support for rooting specific mobile devices, downloading the right files, downgrading if needed, interaction guidance. Diagnostics. Pre-check to see if device is rootable, and to what degree, what works what is broken. Use of trusted images and ROMs. Target platform is Windows, Linux and MacOs with python 2.7+.

## Background
Rooting is complicated, it's based on guides spread across the internet. The guides are manual, some a semi-automated, all of them does not target current versions. I ran into this issue when trying to root a phone, the guide was confusing, I had to manually download files, and in the end I was not able to root because my Android ROM (The UI) had removed a component, and the only path was to downgrade to the version used in the guide. While looking for the older version, I accedentially trusted developers for apps that I don't know what was doing and I had to wipe my laptop as it probably had been compromised. The reason I needed root was Verizon bloatware is blocking page plus tethering (hotspot). I was paying for hotspot, but it was blocked by Verizon app.

## Vision

Uncomplicated Root (uroot) shall be the most popular method to root a phone on the three popular platforms. It shall minimize the time spent on rooting a phone. It shall be public domain. uroot community and documentation, support forum shall be moderated by community specialists to avoid spam and off topic comments. We don't have 20,000+ devices and versions to test and configure, so uroot will depend on community specialists, who will send feedback on successfull steps to root a specific device, with an specific Android version/build. 

## Anology

If you are familiar with ufw (Uncomplicated Firewall), you know how simple it is compared to the underlying iptables commands. uroot takes the same approach by wrapping complicated adb commands, downloading etc into a module called uroot.

## Usage

Install python 2.7+ on your windows, macos or Linux.
Install the uroot module

```
pip install uroot
```

Run the uroot, and create project folder

``` 
python uroot myproject
```

The program will guide you through a series of steps, to install dependencies, e.g. adb, it will assess if your device and it's current software can be rooted, and if it can be rooted what will work, and what will break. It will then do a deeper analysis of connectivity to the device. 





