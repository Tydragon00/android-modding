# android-modding
Script for modding android devices



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
       
    
- Install custom ROM
  - Reboot device in custom recovery
    ```console
    $ adb reboot recovery
  - Open adb sideload from device
  - Intsall custom rom with sideload
    ```console
    $ adb sideload  "ROM file.zip" 
 
  
# For Samsung devices (odin mode):
  - Install custom recovery (TWRP or OrangeFox)
    - Reboot in fastboot
      ```console
      $ adb reboot bootloader

    - "Inserire parte mancante"
    - Install custom recovery
      ```console
      $ heimdall flash --RECOVERY recovery.img
  


