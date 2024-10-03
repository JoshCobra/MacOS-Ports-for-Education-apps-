# PREVIEW

I'm currently working on porting Proteus 8 Professional to MacOS. I’ve successfully managed to get the application running quite smoothly, but it still requires some additional configuration to function optimally. Along the way, I’ve encountered some limitations that I would mention at the end of this md

## Instructions 

### Requirements 
- Wineskin Winery installed, *quick installation using homebrew:*
  ```
  brew install --cask --no-quarantine gcenx/wine/wineskin
  ```
- Microsoft Visual C++ 2008, 2010, 2013, 2015 Runtime Libraries
   - The Proteus 8 Installer usually comes with these installations   
  
- Create the Wrapper using wineskin (recommended version WineskinCX 23.7.1)
  
- .NET libraries might be required for the application to work properly, especially since the latest versions of .NET are no longer readily available through Wineskin services, so I’ve extracted the necessary files from a Windows device as well: `C:\Program Files (x86)\Microsoft.NET`
   - Put these libraries on:
     ```
     /Wineskin/Proteus 8 Professional.app/Contents/SharedSupport/prefix/drive_c/Program Files (x86)
     ```
  
- *Copy of Proteus 8 Professional (v.8.13 tested)*

### Installation
1. Navigate to your Proteus 8 Installer, *(tested using the Proteus 8.13 Version)*
2. Run the `installer.exe` of proteus
3. Select the `C:\Program Files (x86)\Labcenter Electronics\Proteus 8 Professional` path, and let the installer run
4. When finished open proteus
  - Introduce your license
5. Close Proteus and navigate to your installation
  ```
  /Wineskin/Proteus 8 Professional.app/Contents/Wineskin.app
  ```
  - Open the `Wineskin.app`
        ![wineskin.app](https://github.com/user-attachments/assets/a4c649dc-f88f-4202-80d6-5e3a6af1fe0f)
      - Select the `Advanced` tab and then `Winetricks`
        ![Advanced](https://github.com/user-attachments/assets/ab02c5a8-c603-4d46-a6a0-c96dbc35cbbc)

      - Open the `settings` tab, search for the `vidememorysize=4`, and hit run, you should get:
        ```
        Executing load_videomemorysize 4096
        Setting video memory size to 4096
        Executing wine C:\windows\syswow64\regedit.exe /S C:\windows\Temp\set-video.reg
        Executing wine C:\windows\regedit.exe /S C:\windows\Temp\set-video.reg
        ```
        ![Executing load_videomemorysize 4096](https://github.com/user-attachments/assets/28325550-62a4-4e65-95e9-2a265c75d41e)
      - Close and `test run`
6. You now should have the program running correctly
        ![Runnin Program](https://github.com/user-attachments/assets/5606b9b6-efbe-4105-a961-7479e055920c)

### Limitations

I've encountered some limitations of power, when loading big projects it freezes, making it hard to work on
and also with the inputs from the Mac, like the touchpad not working as expected.
- If you find more issues, pls post them in the `issues` tab
- commit and feel free to contribute to this port.

