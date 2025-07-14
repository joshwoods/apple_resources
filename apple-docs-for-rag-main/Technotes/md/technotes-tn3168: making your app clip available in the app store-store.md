

- Technotes
-  TN3168: Making your App Clip available in the App Store 

Article

# TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

## Overview

An App Clip is a lightweight version of your app that lets people quickly start and finish a task from your app, without downloading and installing it. People launch your App Clip by performing an invocation, for example, by scanning an App Clip Code at a physical location, tapping a link in the Maps app, or tapping an App Clip preview. To configure how your App Clip is launched, you create a default App Clip experience and optional advanced App Clip experiences in App Store Connect. To learn how to configure, build, test, and distribute an App Clip, see App Clips.

When you launch a debug or release build of your App Clip, you may discover that your App Clip fails to launch with the following error message:

```
This app clip is not currently available in your country or region
```

This error can occur in the following scenarios:

- The device has connectivity issues.

- The app is unavailable in the storefront associated with the Apple ID currently logged into the device.

- The App Clip uses unexpected configurations.

If your device has connectivity issues, wait until your network conditions improve to launch your App Clip again.

A customer’s Apple ID country or region determines the App Store country or region where they can purchase or download apps. For example, an Apple ID set to France can only purchase apps from the App Store in France. In App Store Connect, you can select the countries or regions where your app is available on the App Store. For more information, see Manage availability for your app on the AppStore. Your App Clip is available anywhere your app is on the App Store. Before launching your App Clip on a device, confirm that your app is available in the country or region associated with the Apple ID currently logged into the device. For example, if your app is available in all countries or regions of the App Store except France, launching your App Clip on a device with an Apple ID set to France will fail with the above message.

Once you have a stable network and set up your app’s availability in App Store Connect, log in to your device with an Apple ID set to a country or region where your app is available, then perform an invocation. If your App Clip still fails to launch with the above message, review this document to find out how you can properly configure your App Clip for testing and App Store distribution.

## Use a bundle ID registered in App Store Connect

You register a bundle ID for your App Clip when you upload the first build of your app that contains an App Clip to App Store Connect. You can’t change it after uploading your first build. Use this bundle ID anywhere you need to identify your App Clip, for example, when you change the bundle identifier field in the General pane of your App Clip’s target in Xcode or when you define a default App Clip link for your local App Clip experience.

After you update your App Clip, create a release build of your app that includes it, then inspect the `.ipa` file of your app. Confirm that the bundle ID in the `Info.plist` file of your released App Clip matches your registered bundle ID. To inspect an `.ipa` file, follow the instructions in Identify and remove unused assets. To learn how to create a release build of your app, see Testing a release build.

## Set up your advanced App Clip experience with an approved place association

To create an advanced app Clip experience that appears in Apple Maps, you define a place association that connects the App Clip experience to a physical location in App Store Connect. Set the place association to a location approved for your business on Apple Maps. For more information, see set up an advanced App Clip experience with place association.

## Avoid using the Enterprise distribution method

Enterprise distribution isn’t available to App Clips. To distribute your App Clip to registered devices, use the Ad Hoc or Development method. To distribute an app that includes your App Clip to testers or on the App Store, use the App Store method. For more information about available distribution options, see Distributing your app for beta testing and releases.

## Cache your App Clip before testing your local experience

To test your App Clip with a local experience, build your App Clip, sign it for Development, Ad Hoc, or TestFlight distribution, then run your App Clip on your test device to cache it. Local experiences don’t launch an App Clip that’s published on the App Store. For more information, see Testing the launch experience of your App Clip.

## Clear the cache before testing your advanced App Clip experiences

To show new or updated App Clip experiences, clear the cache on your device before performing invocations for your advanced App Clip experiences. For more information, see Testing the launch experience of your App Clip.

## Retry your invocation later

In rare cases, your App Clip may become unavailable due to factors outside of your control. After Apple approves your App Clip, it may unexpectedly take some time for your App Clip to be available in all the countries or regions you select in App Store Connect. The same situation may occur when you edit your App Clip information in App Store Connect. Retry your invocation at a later time.

## Revision History

- **2024-06-04** First published.

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

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

