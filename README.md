# Development Environment Lab

## Description:
This Readme explains how to set up a development environment using a virtual machine, through using Vagrant and VirtualBox.

## How to do:
1. Download both Vagrant and VirtualBox.

2. Make a folder that you will use to place all the code into, e.g. Vagrant_DevEnv.

3. Enter the folder in the command line and type 'vagrant init 'ubuntu/*file name*' '.

4. Open the folder in your chosen text editor, e.g. if you are using Atom, type 'atom .' into your command line.

5. Remove all the commented code from the vagrantfile.

6. Go back into command line and type 'vagrant up' - this will create the virtual machine.

7. Then, type 'vagrant ssh' into the command line to give you access to a shell.

8. We must now update the virtual machine, so type 'sudo apt-get update && apt-get upgrade -y' into your command line.

9. To initiate the server, type in 'sudo apt-get install nginx -y'.

10. Type 'ifconfig' in the command line to find what the address is of your development environment (it is labelled as 'inet addr'), and copy it to your clipboard.

11. You can test if your server is up by typing 'curl' followed by the address you just copied into the command line. If it is working, it will display your server's contents in the command line in code form.

12. In your browser type 'http://' followed by the address that you copied from 2 steps ago.

13. If you make any changes in your vagrantfile, then you have to re-enter the folder in the command line and type 'vagrant reload'. After this, you then have to repeat steps 6 to 11.
