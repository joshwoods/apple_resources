

- Background Assets
-  Downloading essential assets in the background 

Sample Code

# Downloading essential assets in the background

Fetch the assets your app requires before its first launch using an app extension and the Background Assets framework.

Download

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 18.4+visionOS 2.4+Xcode 15.0+

## Overview

Note

This sample code project is associated with WWDC23 session 10108: What’s new in Background Assets.

### Configure the sample code project

Before you run the sample code project in Xcode:

- Configure the WWDC Sessions and WWDC Sessions Background Assets Extension targets to use your Developer team for signing.

- See Assign a project to a team.

## See Also

### Asset download management

class BADownloadManager

An object that manages the queue of scheduled asset downloads.

protocol BADownloaderExtension

An interface for reacting to app life-cycle events and processing concluded asset downloads while your app isn’t running.

protocol BADownloaderExtensionConfiguration

