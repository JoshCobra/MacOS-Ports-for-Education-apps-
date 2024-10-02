# MacOS-Ports-for-Education-apps-

### - Check The Releases Section

The aim of this repository is to port educational applications from Windows to MacOS, focusing on software that is either 
unavailable natively for MacOS or performs better in a Windows environment. 
These efforts are targeted at improving access to essential educational tools for MacOS users.

This project leverages my knowledge of both operating systems and contributions from the open-source community.
To achieve these ports, I am using Wineskin as the foundational tool to facilitate the process of running Windows applications on MacOS.
More details on Wineskin can be found in the official repository:
- WineskinServer by Gcenx. https://github.com/Gcenx/WineskinServer

Note on Compatibility: Achieving these ports is generally more straightforward on Intel-based MacBooks, as they share a similar architecture with Windows PCs, making the process of running Windows applications through emulation or translation layers more efficient. For MacBooks with Apple Silicon (M1, M2), additional layers like Rosetta 2 or alternative solutions may be required, but these systems can still be supported with the appropriate adjustments.

Windows-Only Packages: Some Windows applications require specific libraries or frameworks, such as .NET, which may not be as easily accessible for download as they once were. However, these packages are still essential for the proper functioning of many educational tools. In such cases, alternative methods to obtain and integrate these components into the MacOS environment can be used. These frameworks can typically be installed manually or through third-party solutions to ensure compatibility.

Additionally, various add-ons and configurations may be required to ensure the proper functioning of the ported applications.

If a similar project already exists or if you have relevant expertise, I encourage you to reach out. 
I am open to collaboration or, if necessary, ensuring proper attribution of existing work.

Disclaimer:
I do not claim ownership of any of the software or archives used in this project. 
This project is purely for educational purposes, and all software remains the property of their respective owners.
Please ensure that you use appropriate licenses, keys, and activation codes where required.

### Components that fall under LGPL-2.1 license

`Wineskin Winery.app`
`Wineskin.app`
`wineskinlauncher`

The license is kept the same as the original material as LGPL 2.1. You can find more details in the [LICENSE](https://github.com/JoshCobra/MacOS-Ports-for-Education-apps-/blob/main/LICENSE) file.



