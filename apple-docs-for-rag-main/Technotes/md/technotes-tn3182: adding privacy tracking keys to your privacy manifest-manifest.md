

- Technotes
-  TN3182: Adding privacy tracking keys to your privacy manifest 

Article

# TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

## Overview

When you build an app or third-party SDK that contacts domains engaged in tracking, perform these steps in your privacy manifest (`PrivacyInfo.xcprivacy`):

1.  Add the `NSPrivacyTracking` key and set its value to `true`.

2.  Add the `NSPrivacyTrackingDomains` key and set its value to a list of tracking domains.

For more information about these keys and the privacy manifest, see Privacy manifest files.

This document describes how to add the `NSPrivacyTracking` and `NSPrivacyTrackingDomains` keys to your privacy manifest in Xcode. If you work outside of Xcode, review this document to learn about the expected structure of each key.

Note

Before you start adding the keys to your privacy manifest, enable raw keys and values in Xcode to view the raw keys and hide their human-readable names. Click anywhere in the privacy manifest, then choose Xcode \> Editor \> Raw Keys and Values. Repeat the process to disable this feature.

## Add the privacy tracking key

The `NSPrivacyTracking` key uses the following format:

```
NSPrivacyTracking
 if your app or third-party SDK contacts domains engaged in tracking; otherwise use 
    . -->

```

To add the `NSPrivacyTracking` key to your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Click the Add button (+) beside the `App Privacy Configuration` key in the property list editor.

3.  In the pop-up menu that appears, choose `NSPrivacyTracking`.

4.  Confirm the value is `Boolean` in the Type column.

5.  Select `YES` from the pop-up menu in the Value column.

## Add a tracking domain to the privacy tracking domains key

Set the value of the `NSPrivacyTrackingDomains` key to a list of tracking domains in your privacy manifest. For more information about tracking domains, see “Configure a tracking domain” in TN3181: Debugging an invalid privacy manifest.

To add a tracking domain to the `NSPrivacyTrackingDomains` key in your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Find the `NSPrivacyTrackingDomains` key in the property list editor.

3.  Confirm the value is `Array` in the Type column.

4.  Click the disclosure triangle to the left of `NSPrivacyTrackingDomains` to reveal it.

5.  Click the Add button (+) beside `NSPrivacyTrackingDomains` to insert a tracking domain such as `mywebsite.example.com`.

## Add the privacy tracking domains key

The `NSPrivacyTrackingDomains` key uses the following format:

```
NSPrivacyTrackingDomains

    mywebsite.example.com
    ...

```

Each string value in the array identifies an internet domain your app or third-party SDK connects to that engages in tracking. For more information, see Add a tracking domain to the privacy tracking domains key.

To add the `NSPrivacyTrackingDomains` key to your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Click the Add button (+) beside the `App Privacy Configuration` key in the property list editor.

3.  In the pop-up menu that appears, choose `NSPrivacyTrackingDomains`.

4.  Confirm the value is `Array` in the Type column.

5.  To add a tracking domain to the array, see Add a tracking domain to the privacy tracking domains key.

The following example declares one tracking domain for an app called `Sample`:

- Source code
- Property list

```

    NSPrivacyTracking

    NSPrivacyTrackingDomains

        mywebsite.example.com

```

Repeat step 5 for each additional tracking domain your app or third-party SDK contacts. The example below declares an additional tracking domain for `Sample`:

- Source code
- Property list

```

    NSPrivacyTracking

    NSPrivacyTrackingDomains

        mywebsite.example.com
        tracking.subdomain.example.com

```

## Revision History

- **2024-12-17** First published.

## See Also

### Latest

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

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

