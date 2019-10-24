# **Installing Kali Linux on VirtualBox (pre-made image method)**

**Installing VirtualBox**

1.  Navigate to <https://www.virtualbox.org> and download VirtualBox the
    installer for your operating system

2.  Run the installer and complete the setup. You can accept all the defaults.

**Downloading the Kali Image**

[Download VirtualBox Image 64-bit](https://images.offensive-security.com/virtual-images/kali-linux-2019.3a-vbox-amd64.ova)

**Setting Up the Virtual Machine**

1.  Open VirtualBox

2.  Click “Import”

3.  Choose the virtual appliance file to import

    1.  This is the Kali image you just downloaded

4.  Click “Next”

5.  You can leave the defaults and click “Import”

    1.  If you have a lot of RAM or CPU cores, you can adjust the defaults

    2.  You can also change these settings later

6.  Select the virtual machine and click “Start”

    1.  If your machine does not start, go back to
        <https://www.virtualbox.org/wiki/Downloads> and download VirtualBox
        6.0.12 Oracle VM VirtualBox Extension Pack

    2.  Open the Extension Pack and click “Install”

    3.  Start the Virtual Machine again

**Logging In and Updating Software**

1.  Username: root

2.  Password: toor

3.  If your computer has a high-resolution screen and the objects on the screen
    are small, you may want to adjust the scaling to make it easier to see
    things

    1.  Click the down arrow on the top right of the screen

    2.  Click the circular settings icon

    3.  Click “Devices” then “Displays”

    4.  I used 200% scaling, just make sure you are setting this value while in
        full-screen mode

        1.  When switching to full-screen mode, make sure to note how to leave
            full-screen from the dialog box that will pop up

            1.  By default, it is ‘right ctrl + f’ to exit full-screen

4.  To update all installed packages, you can run the following command

    1.  sudo apt-get update && apt-get upgrade -y

        1.  This may take a while

        2.  Accept any defaults and press enter key if prompted

5.  You should be up and running now. If you choose to, you can also install
    VirtualBox Guest Addons (I will write up a tutorial on this later)
