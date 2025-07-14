

- Technotes
-  TN3184: Adding data collection details to your privacy manifest 

Article

# TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

## Overview

When you build an app or third-party SDK that collects any data type, perform these steps in your privacy manifest (`PrivacyInfo.xcprivacy`):

1.  Add the `NSPrivacyCollectedDataTypes` key.

2.  For each data type your app or third-party SDK collects, add a dictionary as a value for the `NSPrivacyCollectedDataTypes` key. The dictionary includes the data type, the data linked to the user and tracking status, and a list of reasons for collecting this data type. For more information, see Add a collected data type and reasons dictionary.

For more information about the privacy manifest and these keys, see Privacy Manifest files and Describing data use in privacy manifests.

This document describes how to add the `NSPrivacyCollectedDataType`, `NSPrivacyCollectedDataTypeLinked`, `NSPrivacyCollectedDataTypeTracking`, and `NSPrivacyCollectedDataTypePurposes` keys to your privacy manifest in Xcode. If you work outside of Xcode, review this document to learn about the expected structure of each key.

Note

Before you start adding the keys to your privacy manifest, enable raw keys and values in Xcode to view the raw keys and hide their human-readable names. Click anywhere in the privacy manifest, then choose Xcode \> Editor \> Raw Keys and Values. Repeat the process to disable this feature.

## Add a collected data type key

The `NSPrivacyCollectedDataType` key uses the following format:

```
NSPrivacyCollectedDataType
NS_PRIVACY_COLLECTED_DATA_TYPE_VALUE
```

The `NS_PRIVACY_COLLECTED_DATA_TYPE_VALUE` string specifies the type of data your app or third-party SDK collects. For possible values, see “Report the categories of data your app or third-party SDK collects“ in Describing data use in privacy manifests.

To add the `NSPrivacyCollectedDataType` key to a privacy collected data type and reasons dictionary in your privacy manifest:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Click the Add button (+) beside the dictionary to add a new item.

4.  In the pop-up menu, choose `NSPrivacyCollectedDataType`.

5.  In the Type column, confirm that the value is `String`.

6.  Select a data type from the pop-up menu in the Value column. For possible values, see “Report the categories of data your app or third-party SDK collects“ in Describing data use in privacy manifests.

7.  Confirm that the value exactly matches the type of data your app or third-party SDK collects.

## Add a collected data type linked key

The `NSPrivacyCollectedDataTypeLinked` key uses the following format:

```
NSPrivacyCollectedDataTypeLinked
 if your app or third-party SDK links this data type to the user’s identity; otherwise,
     use . -->

```

To add the `NSPrivacyCollectedDataTypeLinked` key to a privacy collected data type and reasons dictionary in your privacy manifest:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Click the Add button (+) beside the dictionary to add a new item.

4.  In the pop-up menu, choose `NSPrivacyCollectedDataTypeLinked`.

5.  In the Type column, confirm that the value is `Boolean`.

6.  Select `YES` from the pop-up menu in the Value column if your app or third-party SDK links this data type to the user’s identity; otherwise, select `NO`.

## Add a collected data type tracking key

The `NSPrivacyCollectedDataTypeTracking` key uses the following format:

```
NSPrivacyCollectedDataTypeTracking
 if your app or third-party SDK uses this data type to track; otherwise, use . -->

```

To add the `NSPrivacyCollectedDataTypeTracking` key to a privacy collected data type and reasons dictionary in your privacy manifest:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Click the Add button (+) beside the dictionary to add a new item.

4.  In the pop-up menu, choose `NSPrivacyCollectedDataTypeTracking`.

5.  In the Type column, confirm that the value is `Boolean`.

6.  Select `YES` from the pop-up menu in the Value column if your app or third-party SDK uses this data type to track; otherwise, select `NO`.

## Add a collected data type purposes key

The `NSPrivacyCollectedDataTypePurposes` key uses the following format:

```
NSPrivacyCollectedDataTypePurposes

    NS_PRIVACY_COLLECTED_DATA_TYPE_PURPOSE_VALUE
    ...

```

Each `NS_PRIVACY_COLLECTED_DATA_TYPE_PURPOSE_VALUE` string in the array identifies a reason why your app or third-party SDK collects a data type. For possible values, see “Report the reasons your app or third-party SDK collects data” in Describing data use in privacy manifests.

To add the `NSPrivacyCollectedDataTypePurposes` key to a privacy collected data type and reasons dictionary in your privacy manifest:

1.  Select the dictionary in the property list editor.

2.  Click the disclosure triangle to the left of the dictionary to reveal it.

3.  Confirm the dictionary contains a `NSPrivacyCollectedDataType` key with a value as described in Add a collected data type key.

4.  Click the Add button (+) beside the dictionary to add a new item.

5.  In the pop-up menu, choose `NSPrivacyCollectedDataTypePurposes`.

6.  In the Type column, confirm that the value is `Array`.

7.  Click the disclosure triangle to the left of `NSPrivacyCollectedDataTypePurposes` to reveal it.

8.  Click the Add button (+) beside `NSPrivacyCollectedDataTypePurposes` to add a reason.

9.  Choose a reason from the pop-up menu in the Value column. For possible values, see “Report the reasons your app or third-party SDK collects data” in Describing data use in privacy manifests.

Repeat the last two steps for each reason your app or third-party SDK collects this data type.

## Add a collected data type and reasons dictionary

A privacy collected data type and reasons dictionary includes a data type, a data linked to the user status, a tracking status, and a list of reasons for collecting this data type. The dictionary contains exactly four keys: `NSPrivacyCollectedDataType`, `NSPrivacyCollectedDataTypeLinked`, `NSPrivacyCollectedDataTypeTracking`, and `NSPrivacyCollectedDataTypePurposes`. It uses the following format:

```

    NSPrivacyCollectedDataType
    NS_PRIVACY_COLLECTED_DATA_TYPE_VALUE

    NSPrivacyCollectedDataTypeLinked

    NSPrivacyCollectedDataTypeTracking

    NSPrivacyCollectedDataTypePurposes

        NS_PRIVACY_COLLECTED_DATA_TYPE_PURPOSE_VALUE
        ...

```

To add a privacy collected data type and reasons dictionary to the `NSPrivacyCollectedDataTypes` key in your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator in Xcode.

2.  Find the `NSPrivacyCollectedDataTypes` key in the property list editor.

3.  Click the disclosure triangle to the left of `NSPrivacyCollectedDataTypes` to reveal it.

4.  Click the Add button (+) beside `NSPrivacyCollectedDataTypes` to insert a new item.

5.  Confirm the value is `Dictionary` in the Type column.

6.  Click the disclosure triangle to the left of the dictionary to reveal it.

7.  To add the `NSPrivacyCollectedDataType` key to the dictionary, see Add a collected data type key.

8.  To add the `NSPrivacyCollectedDataTypeLinked` key to the dictionary, see Add a collected data type linked key.

9.  To add the `NSPrivacyCollectedDataTypeTracking` key to the dictionary, see Add a collected data type tracking key.

10. To add the `NSPrivacyCollectedDataTypePurposes` key to the dictionary, see Add a collected data type purposes key.

## Add the collected data types key

The `NSPrivacyCollectedDataTypes` key is an array of privacy collected data type and reasons dictionaries. For more information, see Add a collected data type and reasons dictionary. The key uses the following format:

```
NSPrivacyCollectedDataTypes

        NSPrivacyCollectedDataType
        NS_PRIVACY_COLLECTED_DATA_TYPE_VALUE

        NSPrivacyCollectedDataTypeLinked

        NSPrivacyCollectedDataTypeTracking

        NSPrivacyCollectedDataTypePurposes

            NS_PRIVACY_COLLECTED_DATA_TYPE_PURPOSE_VALUE
            ...

    ...

```

To add the `NSPrivacyCollectedDataTypes` key to your privacy manifest:

1.  Select `PrivacyInfo.xcprivacy` in the Project navigator.

2.  Click the Add button (+) beside the `App Privacy Configuration` key in the property list editor.

3.  In the pop-up menu that appears, choose `NSPrivacyCollectedDataTypes`.

4.  Confirm the value is `Array` in the Type column.

5.  To add a privacy collected data type and reasons dictionary, see Add a collected data type and reasons dictionary.

The following example declares the contacts information collected from the user in an app named `Sample`:

- Source code
- Property list

```

    NSPrivacyCollectedDataTypes

            NSPrivacyCollectedDataType
            NSPrivacyCollectedDataTypeContacts
            NSPrivacyCollectedDataTypeLinked

            NSPrivacyCollectedDataTypeTracking

            NSPrivacyCollectedDataTypePurposes

                NSPrivacyCollectedDataTypePurposeAppFunctionality

```

Repeat step 5 for each additional data type your app or third-party SDK collects. In the following example, `Sample` additionally collects user ID information from the user:

- Source code
- Property list

```

    NSPrivacyCollectedDataTypes

            NSPrivacyCollectedDataType
            NSPrivacyCollectedDataTypeContacts
            NSPrivacyCollectedDataTypeLinked

            NSPrivacyCollectedDataTypeTracking

            NSPrivacyCollectedDataTypePurposes

                NSPrivacyCollectedDataTypePurposeAppFunctionality

            NSPrivacyCollectedDataType
            NSPrivacyCollectedDataTypeUserID
            NSPrivacyCollectedDataTypeLinked

            NSPrivacyCollectedDataTypeTracking

            NSPrivacyCollectedDataTypePurposes

                NSPrivacyCollectedDataTypePurposeAnalytics
                NSPrivacyCollectedDataTypePurposeOther
                NSPrivacyCollectedDataTypePurposeProductPersonalization

```

## Revision History

- **2024-12-17** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

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

