Step-by-Step Guide to Boot Linux Ubuntu via Command Line (CLI)
1. Prepare Bootable Media (USB/CD/DVD)
  First, you'll need a bootable Ubuntu USB drive or DVD. If you haven't done so already, download the Ubuntu ISO and create a bootable USB using a tool like Rufus (on Windows) or dd (on Linux).
  Insert the bootable media into your computer.
2. Enter BIOS/UEFI Settings
  Turn on your computer and immediately press the appropriate key to enter BIOS/UEFI settings (this key is typically Esc, F2, F12, or Del depending on the manufacturer).
  In BIOS/UEFI, change the boot order to boot from the USB or DVD drive first.
  Save the changes and exit BIOS.
3. Boot into Ubuntu Installation Media
  Your computer will now boot from the USB or DVD, and you will see the GRUB menu. The GRUB (GRand Unified Bootloader) is the bootloader used by Ubuntu to manage the boot process.
4. Access the Command-Line Interface (CLI)
  In the GRUB menu, you will have a few options:
  Try Ubuntu without installing (to run it live from the USB without affecting the system).
  Install Ubuntu (to begin the installation process).
  Use the arrow keys to select the Try Ubuntu without installing option (this will allow you to access the live session and CLI).
  Once Ubuntu loads, you will be in a live session, and you can use the command line.
5. Open a Terminal Window
  In the live Ubuntu environment, open a terminal by pressing Ctrl+Alt+T or search for “Terminal” in the application menu.
6. Accessing the Ubuntu System via CLI
  Now, you're ready to perform operations via the command line. For example, you can:
Check system info:
`uname -a`
List available disks (if you want to mount an existing Ubuntu system or recover data):
`sudo fdisk -l`
Mount a partition:
  If you want to mount a specific partition (for example, /dev/sda1):
    `sudo mount /dev/sda1 /mnt`
Access system logs:
  For checking system logs:
    sudo less /var/log/syslog
8. Reboot into Installed Ubuntu (If needed)
    If you're in a recovery situation or trying to boot into your existing installation, you may want to reboot directly into the installed system. You can do so via the command line:
        `sudo reboot`
