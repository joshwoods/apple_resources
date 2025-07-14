

- Technotes
-  TN3118: Debugging your app’s launch screen 

Article

# TN3118: Debugging your app’s launch screen

Understand why your app’s launch screen is not displayed or updated.

## Overview

A Launch Screen appears instantly when your app starts up and is quickly replaced with the app’s first screen, giving the impression that your app is fast and responsive. As you upgrade your application’s launch screen you may discover that the old version still appears or that it appears empty. This article explains possible reasons and how to fix them.

## Launch screen does not display properly

Check why your launch screen fails to display:

- **iOS displays an outdated launch screen.** Your new Xcode build has not overwritten the old launch screen. Clean your build folder for your project. In Xcode, select your target, then select the menu Product, menu item Clean Build Folder. Remove the app from device or Simulator. Build and run the app again.

- **iOS displays the last shown view controller.** When your app enters the background, iOS takes a snapshot of the app, and displays the snapshot on subsequent launches. If you want your launch screen to appear again, remove your app from the device, and run it again from Xcode.

For SwiftUI-based or UIKit-based apps that use a launch screen in its Information Property List:

- **Your `Info.plist` is misconfigured**. It is missing the UILaunchScreen key-value, or the UIImageName key-value does match with the image name what is found in the asset catalog. Be aware that case sensitivity is important.

For UIKit-based apps using a Storyboard Launch Screen:

- **The Launch Screen storyboard name doesn’t match what’s in the target settings.** Select your Xcode target, goto the General tab, refer to the ‘App Icons and Launch Images’ section. The Launch Screen File setting should match the name of your launch screen storyboard found in the Project Navigator. To find out more about setting up your Launch Screen in Xcode, refer to Specifying Your App’s Launch Screen.

- **The image in your launch screen storyboard did not originate from the target’s asset catalog.** If you are using static images in your launch screen, check to make sure the image originates from the product’s asset catalog as a JPG or PNG image.

- **Your Launch Screen storyboard’s initial view controller scene is not set as the initial view controller**. Xcode will warn you: “Warning: Unsupported Configuration: ‘View Controller’ is unreachable because it has no entry points”. Select the view controller scene in your launch screen storyboard. Make sure Is Initial View Controller is checked.

Note

If you are using a 3rd party development environment that provides the launch screen for your app, contact that 3rd party support team for help.

## App launching with state restoration

Implement state restoration in your app so that the launch screen is used less often. iOS snapshots your app when it’s suspended and may use this snapshot instead of the launch screen the next time the app is launched. Users expect your app to be in the same state as when they left it. For more information on state restoration refer to About the UI Restoration Process.

## Revision History

- **2023-07-25** Fixed some broken links.

- **2022-05-24** Made minor editorial changes.

- **2022-03-01** First published.

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

