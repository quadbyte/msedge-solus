# Microsoft Edge Dev for Solus

<!-- # Archived
I am no longer willing to maintain the packages to the latest version as I no longer use them.  
You can use this as the template of your repo and maintain if you want. -->

## Disclaimer
These packages are **not official**, they are neither supported nor endorsed by the official Solus devs or MSEdge devs. Do not ask for help in Solus's/Microsoft's help forum, instead create an issue [here](https://github.com/GZGavinZhao/msedge-solus/issues). 

I do **NOT** have the source code for Microsoft Edge. This installation file is created by simply decompressing official the .deb installation file and copying/assigning its contents to the right location(s) your Solus system.

## Direct .eopkg files
Now you can directly download the compiled .eopkg files from [here](https://github.com/GZGavinZhao/msedge-solus/releases/latest)

To install any program directly from eopkg file, First download the file and then `cd` into that folder like `$ cd ~/Downloads`, After that run  
```
$ sudo eopkg it ./your-program-name.eopkg
```
**NOTE** : Please read the release notes first to know if there are any extra dependencies or not.

### Building from Source
```
$ sudo eopkg bi --ignore-safety https://raw.githubusercontent.com/GZGavinZhao/msedge-solus/main/browser/microsoft-edge-dev/pspec.xml && sudo eopkg it microsoft-edge-dev*.eopkg && sudo rm microsoft-edge-dev*.eopkg
```
**NOTE** In order to use the latest sign-in and sync support for version 91.0.831.1 and above, after installation you might need to manually type `edge://flags` in the address bar, then search for and enable the "MSA sign in" experiment.
