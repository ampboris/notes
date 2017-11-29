## INSTALL NODE-SASS and node-gyp etc:

npm install --global --production windows-build-tools

The config steps with Node.js should now be as follows:

1. Install [Visual C++ 2015 Build Tools] - VC++ Build Tools Technical Preview], choose Custom Install, and select both Windows 8.1 and Windows 10 SDKs.

	* [Windows 7 only] requires .NET Framework 4.5.1

2. Install Python 2.7, and add it to your PATH
3. npm config set python python2.7
4. Launch cmd, npm config set msvs_version 2015 --global 
		(this is instead of npm install [package name] --msvs_version=2015 every time.)

5. SO MUCH npm install
6. FIX: in windows and behind proxy, err => Cannot download "win32-x64-48_binding.node"
	Download https://github.com/sass/node-sass-binaries/blob/master/win32-x64-48_binding.node
	And put it in a directory.
	SET SASS_BINARY_PATH=C:\Development\win32-x64-48_binding.node
  
  ## SWAGGER Node express!
