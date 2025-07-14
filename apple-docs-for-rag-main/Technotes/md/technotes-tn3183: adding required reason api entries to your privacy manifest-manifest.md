

- Technotes
-  TN3183: Adding required reason API entries to your privacy manifest 

Article

# TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

## Overview

When you build an app or third-party SDK that uses any required reason API, perform these steps in your privacy manifest (`PrivacyInfo.xcprivacy`):

1.  Add the `NSPrivacyAccessedAPITypes` key and set its value to the dictionary.

2.  For each required reason API your app or third-party SDK uses, add a dictionary as a value for the `NSPrivacyAccessedAPITypes` key. The dictionary includes the category of the reason API and a list of reasons for using this API. For more information, see Add an accessed API type and reasons dictionary.

See Privacy Manifest files and Describing use of required reason API for more information about the privacy manifest and these keys.

This document describes how to add the `NSPrivacyAccessedAPIType`, `NSPrivacyAccessedAPITypeReasons`, and `NSPrivacyAccessedAPITypes` keys to your privacy manifest in Xcode. If you work outside of Xcode, review this document to learn about the expected structure of each key.

Note

Before you start adding the keys to your privacy manifest, enable raw keys and values in Xcode to view the raw keys and hide their human-readable names. Click anywhere in the privacy manifest, then choose Xcode \> Editor \> Raw Keys and Values. Repeat the process to disable this feature.

## Select an accessed API category

A privacy accessed API category identifies the category of required reason APIs your app or third-party SDK uses. Set the value of the `NSPrivacyAccessedAPIType` key to a privacy accessed API category. For more information, see Describing use of required reason API.

The possible values of a privacy accessed API category are:

- `NSPrivacyAccessedAPICategoryActiveKeyboards`

- `NSPrivacyAccessedAPICategoryDiskSpace`

- `NSPrivacyAccessedAPICategoryFileTimestamp`

- `NSPrivacyAccessedAPICategorySystemBootTime`

- `NSPrivacyAccessedAPICategoryUserDefaults`

## Add an accessed API type key

The `NSPrivacyAccessedAPIType` key uses the following format:

```
NSPrivacyAccessedAPIType
NS_PRIVACY_ACCESSED_API_CATEGORY_VALUE
```

The `NS_PRIVACY_ACCESSED_API_CATEGORY_VALUE` string represents a privacy accessed API category. For more information, see Select an accessed API category.

To add the `NSPrivacyAccessedAPIType` key to a privacy accessed API type and reasons dictionary:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Click the Add button (+) beside the dictionary to add a new item.

4.  In the pop-up menu that appears, choose `NSPrivacyAccessedAPIType`.

5.  Confirm the value is `String` in the Type column.

6.  Select a privacy accessed API category from the pop-up menu in the Value column. For possible values, see Select an accessed API category.

7.  Confirm that the value exactly matches the category of required reason API that your app or third-party SDK uses.

## Add an accessed API type reasons key

The `NSPrivacyAccessedAPITypeReasons` key uses the following format:

```
NSPrivacyAccessedAPITypeReasons

    NS_PRIVACY_ACCESSED_API_TYPE_REASON_VALUE
    ...

```

Each `NS_PRIVACY_ACCESSED_API_TYPE_REASON_VALUE` string in the array identifies a reason why your app or third-party SDK uses a required reason API. All the values in the array are associated with a `NSPrivacyAccessedAPIType` key you provide when you create a privacy accessed API type and reasons dictionary.

To add the `NSPrivacyAccessedAPITypeReasons` key to a privacy accessed API type and reasons dictionary:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Confirm the dictionary contains a `NSPrivacyAccessedAPIType` key with a value as described in Select an accessed API category.

4.  Click the Add button (+) beside the dictionary to add a new item.

5.  In the pop-up menu that appears, choose `NSPrivacyAccessedAPITypeReasons`.

6.  Confirm the value is `Array` in the Type column.

7.  Click the disclosure triangle to the left of `NSPrivacyAccessedAPITypeReasons` to reveal it.

8.  Click the Add button (+) beside `NSPrivacyAccessedAPITypeReasons` to add a reason.

9.  Choose a reason from the pop-up menu in the Value column. For possible values, see Describing use of required reason API.

10. Confirm that the value exactly matches a reason for the `NSPrivacyAccessedAPIType` key you use in step 3.

## Add an accessed API type and reasons dictionary

A privacy accessed API type and reasons dictionary includes a category of required reason APIs and a list of related reasons. The dictionary contains exactly two keys: `NSPrivacyAccessedAPIType` and `NSPrivacyAccessedAPITypeReasons`. It uses the following format:

```

    NSPrivacyAccessedAPIType
    NS_PRIVACY_ACCESSED_API_CATEGORY_VALUE

    NSPrivacyAccessedAPITypeReasons

        NS_PRIVACY_ACCESSED_API_TYPE_REASON_VALUE
        ...

```

To add a privacy accessed API type and reasons dictionary to the `NSPrivacyAccessedAPITypes` key in your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Find the `NSPrivacyAccessedAPITypes` key in the property list editor.

3.  Click the disclosure triangle to the left of `NSPrivacyAccessedAPITypes` to reveal it.

4.  Click the Add button (+) beside `NSPrivacyAccessedAPITypes` to insert a new item.

5.  Confirm the value is `Dictionary` in the Type column.

6.  To add the `NSPrivacyAccessedAPIType` key to the dictionary, see Add an accessed API type key.

7.  To add the `NSPrivacyAccessedAPITypeReasons` key to the dictionary, see Add an accessed API type reasons key.

## Add the accessed API types key

The `NSPrivacyAccessedAPITypes` key is an array of privacy accessed API type and reasons dictionaries. For more information, see Add an accessed API type and reasons dictionary. The key uses the following format:

```
NSPrivacyAccessedAPITypes

        NSPrivacyAccessedAPIType
        NS_PRIVACY_ACCESSED_API_CATEGORY_VALUE
        NSPrivacyAccessedAPITypeReasons

            NS_PRIVACY_ACCESSED_API_TYPE_REASON_VALUE
            ...

    ...

```

To add the `NSPrivacyAccessedAPITypes` key to your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Click the Add button (+) beside the `App Privacy Configuration` key in the property list editor.

3.  In the pop-up menu that appears, choose `NSPrivacyAccessedAPITypes`.

4.  Confirm the value is `Array` in the Type column.

5.  To add a privacy accessed API type and reasons dictionary to the array, see Add an accessed API type and reasons dictionary.

The following example declares disk space required reason API usage in an app named `Sample`:

- Source code
- Property list

```

    NSPrivacyAccessedAPITypes

            NSPrivacyAccessedAPIType
            NSPrivacyAccessedAPICategoryDiskSpace
            NSPrivacyAccessedAPITypeReasons

                B728.1
                E174.1

```

Repeat step 5 for each additional required reason API your app or third-party SDK uses. The example below additionally declares user defaults required reason API usage in `Sample`:

- Source code
- Property list

```

    NSPrivacyAccessedAPITypes

            NSPrivacyAccessedAPIType
            NSPrivacyAccessedAPICategoryDiskSpace
            NSPrivacyAccessedAPITypeReasons

                B728.1
                E174.1

            NSPrivacyAccessedAPIType
            NSPrivacyAccessedAPICategoryUserDefaults
            NSPrivacyAccessedAPITypeReasons

                CA92.1

```

## Revision History

- **2024-12-17** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

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

