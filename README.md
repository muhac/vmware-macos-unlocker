# MacOS Unlocker for VMware Workstation
This repository is forked from [paolo-projects/unlocker](https://github.com/paolo-projects/unlocker) and [paolo-projects/auto-unlocker](https://github.com/paolo-projects/auto-unlocker). &emsp; <sub> (May 14, 2020) </sub>



## [Unlocker 3.0.3](https://github.com/paolo-projects/unlocker/releases/tag/3.0.3)

- **On windows machines, it's easier to use auto-unlocker, you can find it here: https://github.com/paolo-projects/auto-unlocker/releases.**
  *It has not been tested extensively*, so if it doesn't work use the `Unlocker.exe --uninstall` command line option to revert changes and use the tool from down here. On linux machines you need to compile it first so unless you're practical with installing the dependencies and a c++17 compliant g++ it's still easier to use the tool down here.
- **Windows**: download, extract and start *win-install.cmd* as administrator
  *(python distribution bundled inside)*
- **Linux**: download, extract and execute *sudo lnx-install.sh*
  *For Linux users*: make sure you have python 3.0+ installed. If you have errors like "Python not supported" but you are sure have python 3+ installed, change the lines inside of lnx-install.sh from 'python xxxxxxx.py' to 'python3.7 xxxxxxx.py' (if you have python 3.7 installed, otherwise try python3 or other stuff)



## [AutoUnlocker 1.1.0](https://github.com/paolo-projects/auto-unlocker/releases/tag/v1.1)

- **Windows x64**: download Unlocker.zip, extract it to a folder and run. Make sure you don't run it from the archive because the *backup* folder it creates is needed if you want to uninstall it later.
  **Since many users are experiencing problems with patching a particular file, it's highly suggested that you manually kill all vmware-related executables through the task manager before running the patch.**
- **Linux**: there's an experimental deb package included that should work on debian-derived (ubuntu included) systems. it uses the std::experimental::filesystem for compatibility. After install, run `sudo auto-unlocker`
  If it doesn't work, then compile following the [README](https://github.com/paolo-projects/auto-unlocker/blob/v1.1/README.md) instructions and run