

- Technotes
-  TN3108: Viewing the interface of your Swift code 

Article

# TN3108: Viewing the interface of your Swift code

Learn how to navigate to the interface file of a Swift implementation file.

## Overview

Xcode generates an interface file that includes all your source code’s internal and public declarations when using the Assistant editor, the Related Items, or the Navigate menu.

## Using the assistant editor

1.  In the project navigator, select your implementation file.

2.  Choose Editor \> Assistant.

The generated interface for your Swift code appears in the assistant editor on the right. 

## Using the Related Items button

1.  In the project navigator, select your implementation file.

2.  Click the Related Items icon in the editor’s jump bar.

3.  In the menu that appears, choose Counterparts \> \[Filename\] to view your interface file. 

Alternatively, choose Generated Interface \> \[Filename\] from the menu.

To navigate back to your implementation file, choose Original Source from the menu. 

## Using the Navigate menu

In the project navigator, select your implementation file, then choose Navigate \> Jump to Next Counterpart to view the interface file. 

To navigate back to your implementation file, choose Navigate \> Jump to Previous Counterpart or Navigate \> Jump to Original Source \[Filename\]. 

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-02-08** Republished as TN3108 with significant editorial changes.

- **2016-03-23** First published as QA1914.

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

