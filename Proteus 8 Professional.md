# PREVIEW

I'm currently working on porting Proteus 8 Professional to MacOS. I’ve successfully managed to get the application running quite smoothly, but it still requires some additional configuration to function optimally. Along the way, I’ve encountered some limitations that I would mention at the end of this md

## Instructions 

### Requirements 
- Wineskin Winery installed, *quick installation using homebrew:*
  ```
  brew install --cask --no-quarantine gcenx/wine/wineskin
  ```
- Microsoft Visual C++ 2008, 2010, 2013, 2015 Runtime Libraries
  
- Create the Wrapper using wineskin (recommended version WineskinCX 23.7.1)
  
- .NET libraries might be required for the application to work properly, especially since the latest versions of .NET are no longer readily available through Wineskin services, so I’ve extracted the necessary files from a Windows device as well: `C:\Program Files (x86)\Microsoft.NET`
   - Put this libraries
  
- *Copy of Proteus 8 Professional (v.8.13 tested)*


- Navigate to your Proteus 8 Installer, *tested using the Proteus 8.13 Version*
- Run the `installer.exe` of your proteus
- select the `C:\Program Files (x86)\Labcenter Electronics\Proteus 8 Professional` path, and let the installer run
- 
