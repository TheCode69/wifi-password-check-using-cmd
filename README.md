# wifi-password-check-using-cmd
Certainly! Let's go through an example step by step.

1. **Open Command Prompt as Administrator**:
   - Type `cmd` in the Windows search bar.
   - Right-click on "Command Prompt" in the search results.
   - Select "Run as administrator" from the context menu.

2. **View Saved Wi-Fi Profiles**:
   - In the Command Prompt window, type:
     ```
     netsh wlan show profiles
     ```
   - Press Enter.

   This command will list all the Wi-Fi profiles saved on your computer.

3. **Retrieve Wi-Fi Password**:
   - To view the password for a specific Wi-Fi network (for example, a network named "MyWiFiNetwork"), type:
     ```
     netsh wlan show profile name="MyWiFiNetwork" key=clear
     ```
   - Press Enter.

   Look for the "Key Content" field in the output. The value next to "Key Content" is the Wi-Fi password for the specified network ("MyWiFiNetwork" in this case).

Please note that you should replace `"MyWiFiNetwork"` with the actual name of the Wi-Fi network for which you want to retrieve the password. Also, remember that you need administrative privileges to perform these operations.
