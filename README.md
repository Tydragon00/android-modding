# Android-modding
Guide for modding android devices

# Install tool
    $ sudo apt install android-tools-adb android-tools-fastboot -y

# For Xiaomi devices:

- Install custom recovery (TWRP or OrangeFox)
  - Unlock bootloader (with xiaomi tool)
  - adb reboot bootloader ( for restart in fastboot)
  - fastboot flash recovery recovery.img (at the end turn off devices)



- Install custom recovery (TWRP or OrangeFox)
  - Reboot in fastboot
    ```console
    $ adb reboot bootloader
    
  - Unlock bootloader (with xiaomi tool)
  - Install custom recovery
    ```console
    $ fastboot flash recovery recovery.img
  - Reboot on custom recovery
    ```console
    $ fastboot reboot recovery 
       
    
- Install custom ROM
  - Reboot device in custom recovery
    ```console
    $ adb reboot recovery
  - Open adb sideload from device
  - Intsall custom rom with sideload
    ```console
    $ adb sideload  "ROM file.zip" 
 
  


