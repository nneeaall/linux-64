Open Ephys for 64-bit Linux
=======================

This repository contains 64-bit Linux binary files for the Open Ephys GUI. For the source code, see http://github.com/open-ephys/GUI.

It should run on any version of Linux, but so far we've only tested it on Ubuntu and Linux Mint. If you get it to work on another distro, definitely let us know!

This software is still being developed, so we can't guarantee that anything will work as expected. Don't use it for mission-critical data acquisition unless you've thoroughly tested all the features you'll need.

Installation instructions
-------------------------------

1. Download the files from http://open-ephys.org/gui. Or, if you have Git installed on your machine, you can open a Terminal and clone from GitHub: `git clone https://github.com/com/open-ephys-GUI-binaries/linux-64`. The advantage of cloning is that you'll be able to easily keep track of any updates by periodically running `git pull origin master` from the application directory. Otherwise, you'll have to manually download the software (or build it from source) whenever something changes.

2. Drag the "linux-64-master" (downloaded version) or "linux-64" (cloned version) folder to the location of your choice and rename it "Open Ephys"

3. In order to use the GUI with the Open Ephys acquisition board or one of Intan's eval boards, you'll have to update the permissions for external devices. Open a terminal and navigate to the Open Ephys folder, then type `sudo cp 40-open-ephys.rules /etc/udev/rules.d` and hit `ENTER`. You'll have to type your password at this point. Next, type `sudo /etc/init.d/udev restart` and hit `ENTER` again to allow the changes to take effect.

4. Double-click the "open-ephys" application file to run the software.

If you run into problems
-------------------------------

1. READ THE [GUI WIKI](https://open-ephys.atlassian.net/wiki/display/OEW/Open+Ephys+GUI). There's a lot of useful information on the "Tutorial" and "User documentation" pages.

2. If you can consistently replicate the problem, [submit an issue](https://github.com/open-ephys/GUI/issues). You'll need a GitHub account for this, but it's worth signing up for one anyway.

3. As a last resort, [get in touch with us directly](http://open-ephys.org/contact)
