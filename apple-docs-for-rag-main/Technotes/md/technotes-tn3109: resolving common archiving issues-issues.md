

- Technotes
-  TN3109: Resolving common archiving issues 

Article

# TN3109: Resolving common archiving issues

Handle common issues that arise while archiving apps.

## Overview

When you choose Product \> Archive, Xcode creates an archive of your app that will appear in the Archives organizer. If the Archives organizer reports your archive as an app archive, then you can validate or distribute it.

## The Archive command in the Product menu is disabled

You can choose Product \> Archive in Xcode after meeting these requirements:

- You’ve selected a real device or build-only device as the run destination in the scheme building your app. Apps built with simulator SDKs can’t be archived nor submitted to the App Store; see Running Your App in the Simulator or on a Device.

- You’ve enabled the archive action for the scheme building your app. 

## Xcode successfully archived my app, but the archive doesn’t appear in the Archives organizer

Archives appear in the Archives organizer when meeting these requirements:

- Your archive is an app archive. If the Archives organizer reports your archive as generic, read TN3110: Resolving Generic Xcode Archive Issue.

- You’ve selected the `Reveal Archive in Organizer` option in the archive action for the scheme building your app. 

## The Validate Content button is disabled

You have a generic Xcode archive. The Validate Content button is enabled for app archives and disabled for generic ones.  See TN3110: Resolving Generic Xcode Archive Issue for details.

## Unexpected build products and archive methods in the Archive organizer when attempting to distribute my archive

If the Archives organizer offers to distribute your archive’s built product or to export a copy of it, then your archive is likely a generic one.  Read TN3110: Resolving Generic Xcode Archive Issue for information on how to resolve it.

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-02-08** Republished as TN3109 with significant editorial changes.

- **2015-10-15** Updated for Xcode 7.

- **2015-10-14** Updated for Xcode 7.

- **2015-08-18** Made editorial changes.

- **2015-03-27** Updated for Xcode 6.

- **2014-07-17** Fixed typos.

- **2014-03-17** Updated the “Unexpected Save Built Products and Export as Xcode Archive options in the Archives Organizer when attempting to distribute my archive” section.

- **2012-06-28** Added information on how to resolve the Archives Organizer’s “Save Built Products” and “Export as Xcode Archive” issue.

- **2011-09-12** First published as TN2215.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

