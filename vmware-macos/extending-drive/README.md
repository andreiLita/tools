## Resizing MacOSX
In virtual machine settings on hardware hard drive click on expand and set the desired capacity.
Open terminal in MacOSX and type 'diskutil list', you should see this:

![Alt text](workstation.png?raw=true "Workstation")

Write in console 'diskutil apfs resizeContainer /dev/$1 $2GB' , where $1 is the identifier of your disk and $2 is the new size.
Go to diskutility app on MacOSX and partition your drive ( not volume ), and increase the size then apply.
