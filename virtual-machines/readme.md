# Virtual Machines

- Spent too much time having issues with virtualbox and guest additions in both xubuntu and fedora.
- Installed VMware Workstation Pro and fresh xubuntu iso
- Updated and fixed issue with scroll wheel not working when mouse is moving
    - `sudo apt-get install xserver-xorg-input-evdev-dev`
    - `cd /usr/share/X11/xorg.conf.d/`
    - `sudo vim 40-libinput.conf`
    - Change Driver from "libinput" to "evdev"
    - `sudo apt install imwheel`
    - `imwheel -b "4 5"
    - Add command to ~/.bashrc to start automatically 
    ``` 
    # Start imwheel for scrolling fix and silence output:
    imwheel -b "4 5" > /dev/null 2>&1
    ```