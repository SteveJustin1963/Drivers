# Drivers
win 10 fixes


How to Install Unsigned Drivers in Windows 10
 
Each and every hardware device attached to your Windows PC needs hardware drivers in order to work properly. The hardware drivers have low-level access to your Windows system so that they can work as they should. Since the drivers get access to the kernel, Windows requires those drivers to be officially signed. Any driver that doesn’t have the official driver signature from Microsoft will not be allowed to install on Windows.

However, there will be times when you need to install unofficial drivers, unsigned drivers, or even old drivers with no digital signature. In those cases, refer to the instructions below on how to install unsigned drivers in Windows 10. This article will show you three different methods on how to do it, perform the one you find the most comfortable for you.

NOTE: Checking driver signatures is a security feature, and disabling it is not recommended. Only install unsigned drivers from trusted sources.

Installing Unsigned Drivers From Advanced Boot Menu

The easiest way to install unsigned drivers is to use the Windows 10 Advanced Boot menu. To do that:

STEP 1: Press the Windows key + [X] key combination, then navigate to Shut down or sign out.

STEP 2: Press [Shift] + left click on the Restart option.

NOTE: The action above will take you to the Advanced Boot menu.

STEP 3: Under Choose an option, select Troubleshoot.

STEP 4: In the Troubleshoot section, select Advanced options.

STEP 5: Next, select Start-up Settings.

NOTE: The Start-up Settings option will allow you to boot your Windows system in different modes.

STEP 6: Simply click on the Restart button to continue.

STEP 7: Since you will install unsigned drivers, press [F7] on your keyboard to select the 7th option “Disable driver signature enforcement.”

STEP 8: Proceed in installing any unsigned driver you want.

STEP 9: After installing, restart your computer, and the Driver Signature Enforcement will be automatically enabled from the next reboot.

NOTE: If ever you want to install another unsigned driver, you need to go through the above process again.

Installing Unsigned Drivers by Enabling Test Mode

One good thing about this method is that it will stay enabled until you manually turn it off, which is a pretty useful way if you are testing different drivers.

STEP 1: Press the Windows key + [X] to open the Power User menu, then choose the option Command Prompt (Admin).

STEP 2: On the Command Prompt, execute this command: bcdedit /set testsigning on

STEP 3: When a message appears saying that the operation completed successfully, restart your system and you will be booted into Test Mode.

STEP 4: Once you’re in the Test Mode, you can now proceed in installing the unsigned drivers.

NOTE: You will notice a watermark-like information like the one below to indicate that your Windows system is currently in Test Mode.

STEP 5: Once you’re done installing the driver, turn off the Test Mode by executing the following command as an admin: bcdedit /set testsigning off

STEP 6: Reboot your system.

Installing Unsigned Drivers by Disabling Integrity Checks

To disable integrity checks:

STEP 1: Open the Command Prompt as admin from the Power User menu, then execute the command: bcdedit /set nointegritychecks off

STEP 2: After executing the command, restart your PC, and then proceed in installing the unsigned driver for your system.

STEP 3: To re-enable integrity check, execute the below command as an admin in the command prompt: bcdedit /set nointegritychecks on

STEP 4: When you get the message saying the operation was successful, restart your system and you’re good to go.


