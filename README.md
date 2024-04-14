# Creating more insecurities

![image](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/e794e7a4-1714-4560-ab74-f4a30b1c3674)


## Intro

Now I will complete the configurations needed for an authenticated scan.

- In the windows virtual machine, I will disable the User Account control by searching for it in the start menu and click OK.

![VL 30](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/679f80e7-99a7-4beb-9fd3-35e16e7d0904)

- Now I will enable "Remote Registry"
- In the start menu, I typed Services.msc

![VL 31](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/b2886003-b60e-45c1-bbd8-16aaf1c5a724)

- Looked for "Remote Registry" and clicked it.
- I changed the status type to "Automatic"
- Then clicked Apply, then Start, then OK

![VL 32](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/56c4bc17-5e99-4ad9-a5b8-bef1640b333e)

- Now I will set ta "Registry Key"
- In the start menu, I typed Registry Editor and clicked it.

![VL 33](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/47409973-364d-49f5-9ecc-23aa29b5d37b)

- In the Registry Editor, I did the following:
  * Clicked on HKEY_LOCAL_MACHINE
  * Clicked on Software
  * Clicked on Microsoft
  * Clicked on Windows
  * Clicked on CurrentVersion
  * Clicked on Policies
  * Clicked on System Key
 
![VL 34](https://github.com/Ashrafs-Tech/Authenticated-Scan/assets/166546026/b5a019b4-5b3d-4597-aa2b-2014ab971ec8)

- In the System Key, I created a DWORD value.
- I set the value to 1.
- Then closed the Registry Editor.
- Restart the virtual machine

## Step 5 is done
I made the necessary configurations:
- User Account
- Remote Registry
- Registry Key

