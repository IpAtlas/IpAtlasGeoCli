# IpAtlas Command-Line Interface (CLI) Tool
The GeoIp command-line interface (CLI) tool enables you to easily perform IP Lookups, query IP Database Metadata, IP Proxy Database Metadata, and pin databases for extended retention periods beyond the default.
Usage is as simple as installation. Find more information in the documentation below. This tool is designed on the IPAtlas Geolocation platform.

# Installation
Download the `bin/` directory from the GitHub repository. Then, navigate to the `C:/Program Files` directory on your system. Create a new folder named `IpAtlas` and paste the `bin/` folder into it.

To set the environment variable for `C:/Program Files/IpAtlas/bin/geoip.exe`, follow these steps:

1. Right-click on the Windows icon in the taskbar and select "System".
2. In the System window, click on "Advanced system settings" on the left sidebar.
3. In the System Properties window, click on the "Environment Variables..." button.
4. In the Environment Variables window, under "System variables", scroll down and select the "Path" variable, then click on "Edit...".
5. In the Edit Environment Variable window, click on "New" and add the path `C:/Program Files/IpAtlas/bin/` (without including `geoip.exe`).
6. Click "OK" on all windows to save the changes.

Now you should be able to run `geoip.exe` from anywhere in the command prompt without specifying the full path.

# Usage
The first step before using the CLI command features from below is to set a valid context license key. License key is the same value as API Key.
`geoip settings --set-license <LICENSE KEY>`  

How to get a valid license key will be provided soon. If you'd like to get beta access, feel free to contact us on support@ipatlas.net

## Version
You can check CLI version by running the following command: 
`geoip version`

## IP Lookup
Perform IP Address Geolocation lookup.  
`geoip lookup -ip <IP ADDRESS>`

## Query IP Database Metadata
Retrieve information about available IP Database versions:   
`geoip database --get`

To obtain metadata about a specific IP Database version:  
`geoip database --get-version <DATABASE VERSION>` 

## Pin IP Database
To pin the IP Database you want to use for an extended period of time  
`geoip database --pin-database <DATABASE VERSION>`


## Releases
### 1.0.1 - 19/6/2024 
- Updated API Key format 
- Added version command 