

- Xcode
- Devices and Simulator
-  Downloading and installing additional Xcode components 

Article

# Downloading and installing additional Xcode components

Add more Simulator runtimes, optional features, and support for additional platforms.

## Overview

Xcode lets you manage optional components yourself so that you can install only the components you use and remove the ones you don’t. For example, install the Simulator runtimes for the devices and operating systems your app runs on, or add support for platforms that you target. You download and install Xcode components in Xcode settings or using the command line.

Note

Developing for visionOS requires a Mac with Apple silicon.

### Manage Xcode components in settings

To manage your components, choose Xcode \> Settings and click Components in the toolbar. Xcode shows the installed and enabled components along with the amount of storage you can recover if you remove them.

There are three types of components:

Platform Support  
The platforms that you can develop your apps for.

Other Components  
Optional Xcode features you can enable and disable.

Other Installed Platforms  
Simulator runtimes for different devices and OS releases that you can run your app on.

To download and install a component in any of these sections, click the Get button next to the component.

To remove or disable components you no longer use and recover their storage space, select the component and click the Delete button (-) in the lower-left corner. Then click Delete or Disable in the dialog that appears.

You can also install platform support when you create a project by selecting a template and clicking the Get button that appears for platforms that aren’t installed. For more information, see Creating an Xcode project for an app.

Note

You can create a new Xcode project or work with an existing Xcode project on a platform that Xcode is installing, but you can’t run or build the project until Xcode finishes downloading and installing the files.

### Install previously released Simulator runtimes in settings

You can get previously released Simulator runtimes in the Components settings. Click the Add button (+) in the lower-left corner, then select a platform to view a list of its available versions. In the dialog that appears, select one or more versions, and click Download & Install.

### Install Simulator runtimes from the Xcode run destination

When you open an Xcode project for a platform that doesn’t have any installed Simulator runtimes, Xcode displays a Get button next to the run destination. Click the Get button to download and install the most recent Simulator runtime for that platform.

The run destination in your Xcode project indicates when Xcode is downloading a Simulator runtime. You can select a run destination when Xcode completes the download and installation.

### Download Xcode components from the command line

You can also download components in Terminal using the `xcodebuild` command. For example, use the command line to download Xcode components once and then install them across multiple Mac computers.

To download Simulator runtimes for a specific platform, use this syntax:

```
xcodebuild -downloadPlatform  [-exportPath ] [-buildVersion ]
```

For example:

```
xcodebuild -downloadPlatform iOS -exportPath ~/Downloads
```

To specify an OS version, add the `-buildVersion` option:

```
xcodebuild -downloadPlatform iOS -exportPath ~/Downloads -buildVersion 18.0 
```

To download all the supported platforms for the version of Xcode you select, use this syntax with the `-downloadAllPlatforms` option:

```
xcodebuild -downloadAllPlatforms [-exportPath ]
```

### Install downloaded packages from the command line

After you download component packages, you can install them in Terminal with the `xcodebuild` command.

First, select the version of Xcode you want to use with the `xcode-select -s ` command. Next, run `xcodebuild -runFirstLaunch` to install any required system components, including the `simctl` utility. Then, run `xcodebuild` with the `-importPlatform ` option to install the component.

```
xcode-select -s /Applications/Xcode-beta.app
xcodebuild -runFirstLaunch
xcodebuild -importPlatform "~/Downloads/watchOS 9 beta Simulator Runtime.dmg"
```

### Download and install new hardware support in between Xcode releases

To download and install hardware support updates in between Xcode releases, use `xcodebuild` with the `-runFirstLaunch` and `-checkForNewerComponents` options. Before running this command, select the version of Xcode you want to use with the `xcode-select -s ` command.

```
xcode-select -s /Applications/Xcode.app
xcodebuild -runFirstLaunch -checkForNewerComponents
```

If new components exist, the `-checkForNewerComponents` option stores the files in the `~/Library/Developer/Packages/` directory and installs the components for the Xcode version you select.

## See Also

### Simulator management

Installing your app in many Simulator platforms and versions

Set up your app in multiple Simulator platforms and versions without the build-and-run cycle.

