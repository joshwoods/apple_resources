

- Technotes
-  TN3128: Starting SharePlay without an existing FaceTime call 

Article

# TN3128: Starting SharePlay without an existing FaceTime call

Use the share sheet or group activity sharing controller to start SharePlay directly from your app without an existing FaceTime call.

## Overview

With the GroupActivities framework in iOS 15.4 and iPadOS 15.4 and later, you can use the share sheet to start SharePlay experiences directly from your app without an existing FaceTime call.

You can make this same SharePlay experience even better by registering a group activity on an item provider and passing the item provider to the share sheet. Then when you select SharePlay the FaceTime call starts with an activity.

If you don’t use the share sheet, you can implement a custom user interface to bring up the \`GroupActivitySharingController\` and start SharePlay directly from your app without a FaceTime call.

## Display the SharePlay button in the share sheet

An app doesn’t need to adopt any special APIs to display the SharePlay button in the share sheet. If the app has the Group Activities entitlement entitlement, the share sheet displays the SharePlay button automatically. Simply present the share sheet as follows:

```
let shareSheet = UIActivityViewController(activityItemsConfiguration: configuration)
// Present the share sheet.
present(shareSheet, animated: true)
```

For example:

Tap the SharePlay button, and select a person in the people-picker. Then tap the FaceTime button to start a FaceTime call with SharePlay directly from within the app.

## Improve the SharePlay experience in the share sheet

Displaying the SharePlay button in the share sheet as just described allows you to initiate a FaceTime call without an activity to start. You must interact with the app again to pick the content to SharePlay.

You can improve this same SharePlay experience by using registerGroupActivity to register a group activity on the item provider, provide the item provider to the share sheet, and present the share sheet. That way, the FaceTime call starts with an activity.

```
// Register your group activity.
let itemProvider = NSItemProvider()
itemProvider.registerGroupActivity(WatchTogether())

// Provide the item provider to the share sheet.
let configuration = UIActivityItemsConfiguration(itemProviders:[itemProvider])

// Present the share sheet.
let shareSheet = UIActivityViewController(activityItemsConfiguration:configuration)
present(shareSheet, animated: true)
```

Here’s an example implementation:

## Display the SharePlay button less prominently

Tune the presentation behavior of the SharePlay button in the share sheet using the allowsProminentActivity property of the UIActivityViewController. Just set `allowsProminentActivity` to `false` to display the SharePlay button less prominently in the share sheet actions list.

```
let shareSheet = UIActivityViewController(activityItemsConfiguration: configuration)

// Show the SharePlay button less prominently in the share sheet.
shareSheet.allowsProminentActivity = false
```

Here’s how it looks in the share sheet:

## Hide the SharePlay button in the share sheet

If you have some content that isn’t integrated with SharePlay, hide the SharePlay button in the share sheet. Set the excludedActivityTypes property on the `UIActivityViewController` to exclude the SharePlay activity type.

```
let shareSheet = UIActivityViewController(activityItemsConfiguration: configuration)

// Exclude the SharePlay activity in the share sheet.
shareSheet.excludedActivityTypes = [.sharePlay]
```

## Start SharePlay directly from your app’s custom user interface

The `GroupActivitySharingController` presents a view in an app that allows users to start a SharePlay session with selected contacts for a given group activity. For example, a button in an app’s custom user interface can initiate a SharePlay session using the `GroupActivitySharingController`. When the user presses the button, instantiate a `GroupActivitySharingController` with a group activity, then present it. The activity starts automatically with the FaceTime call.

```
// Create a sharing controller for your group activity.
let controller = GroupActivitySharingController(MyActivity())

// Present the sharing controller.
present(controller, animated: true)
```

Once the user initiates the in-app experience, and starts a FaceTime or SharePlay session, they can activate the staged group activity. Once activated, the app receives the group session.

## Revision History

- **2022-09-20** First published.

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

