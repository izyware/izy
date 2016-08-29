# izy
Contains bare minimum commandline interface (< 100Kb) for using the IzyWare application platform. Checkout https://izyware.com for more information.

## INSTALLATION

If you are using npm (the Node.js package manager) always ensure that your npm is up-to-date by running:

`npm update -g npm`  

Then use:

`npm install -g izy`

This will put the `izy` command in your system path, allowing it to be run from any directory.

If you do not have npm or you would rather install the tool locally just download the .zip file from https://izyware.com or clone the git repository.

NOTE: The tool requires stable Node.js versions >= 2.0.0.  

## USING THE TOOL

If you have installed the tool using npm, `izy` will be in your system path and can be run fom any directory. Try:

`izy help`

`izy sysview`

For non npm installations (i.e. downloading the zip file), on windows, use ldo.bat file. On all other platforms (Mac, Unix, etc.) use ldo.sh

So on MacOS or Linux try: `./ldo.sh help`

On Windows based platform use: `./ldo.bat help`

## Module Path Resolution
When an izy command is run from the command line that will have a loadmodule (ldmod) statement, the platform will try to locate the module on the system by searching the local file system for installed Izy packages in the paths defined in thirdparty/config/kernel/extstores/file.js. Notice that these paths are all relative to the full path of the 'izy' command process. To see what the current resolver configuration type:

`izy sysview`

## NOTE
These instructions do not install any packages beyond the command line interface. To recieve help about installing additional packages try the following from the commandline:

`izy help`

or just visit https://izyware.com


