I'm currently working on porting Proteus 8 Professional to MacOS. I’ve successfully managed to get the application running quite smoothly, but it still requires some additional configuration to function optimally. Along the way, I’ve encountered some bugs and limitations, but I believe these issues can be resolved relatively easily.

Current Approach: Instead of using the standard installation program, I directly copied the application's folder from a Windows installation:
C:\Program Files (x86)\Labcenter Electronics\Proteus 8 Professional

Additionally, I suspect that .NET libraries might be required for the application to work properly, especially since the latest versions of .NET are no longer 
readily available through Wineskin services, so I’ve extracted the necessary files from a Windows device as well:
C:\Program Files (x86)\Microsoft.NET

I’m not entirely sure if these .NET components are crucial for the app’s performance on MacOS, but I’ll continue running tests to confirm their importance.

Issues Encountered: One major problem I’ve noticed is with some of the program’s libraries. While they exist in the expected directories, it seems that MacOS’s 
file system sometimes makes these paths inaccessible, as though the system is preventing the correct selection or access through the file browser. 
Despite the libraries being present, MacOS doesn't allow the selection of the correct path, almost as if it’s deliberately blocking access.

## Instructions to Installation

- Create the Wrapper using wineskin (recommended version WineskinCX 23.7.1)
- Navigate to your Proteus 8 Installer for this I'm using the Proteus 8.13 Version
