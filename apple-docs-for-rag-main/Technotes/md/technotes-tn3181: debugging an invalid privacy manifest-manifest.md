

- Technotes
-  TN3181: Debugging an invalid privacy manifest 

Article

# TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

## Overview

Starting November 12, 2024, apps you submit for review in App Store Connect must contain a valid privacy manifest file. If you upload an app to App Store Connect that contains invalid privacy manifest files, you’ll receive an email that includes the name and path of the invalid files in your app bundle. For example:

```
ITMS-91056: Invalid privacy manifest - The PrivacyInfo.xcprivacy file from the following path
is invalid: "PrivacyInfo.xcprivacy". Keys and values in your app's privacy manifests must be
valid. For more details about privacy manifest files, visit: 
https://developer.apple.com/documentation/bundleresources/privacy_manifest_files.
```

An invalid privacy manifest is:

- A property list file that contains invalid keys or values.

- An improperly formatted property list file.

Review Privacy manifest files to learn about the keys you can include in a privacy manifest. This document lists possible reasons for invalid privacy tracking and accessed API values in your privacy manifest. Validate your privacy manifest to determine why your privacy manifest is malformed.

## Configure a tracking domain

A tracking domain is a string that identifies an internet domain your app or third-party SDK connects to that engages in tracking. You set the value of the `NSPrivacyTrackingDomains` key to a list of tracking domains in your privacy manifest. The value of the string meets the following requirements:

- Includes the top-level domain or subdomain.

- Contains no path and query components.

- Contains no trailing slash.

## Possible reason for an invalid tracking value

A value for the `NSPrivacyTracking` key is invalid if the value is any other type than a `Boolean`. In your privacy manifest, change the type of the key to `Boolean`.

## Possible reasons for an invalid tracking domains value

A value for the `NSPrivacyTrackingDomains` key is invalid if the value is any other type than an array of strings. In your privacy manifest, change the type of the key to `Array`, then add one or more tracking domains to the array. For more information, see Configure a tracking domain.

You can create an invalid privacy manifest when you use both `NSPrivacyTrackingDomains` and `NSPrivacyTracking` keys as follows:

| Reason | Solution |
|----|----|
| The value of the `NSPrivacyTracking` key is `true` and the value of the `NSPrivacyTrackingDomains` key is an empty array of strings. | Fill the array with one or more tracking domains your app or third-party SDK connects to. |
| The value of the `NSPrivacyTracking` key is `true` and the value of the `NSPrivacyTrackingDomains` key is an array of strings, but some entries are improperly formatted. | Confirm you configure each tracking domain in the array as described in Configure a tracking domain. |
| The value of the `NSPrivacyTracking` key is `false` and the `NSPrivacyTrackingDomains` key contains some entries. | Remove the `NSPrivacyTrackingDomains` key from your privacy manifest. |

Note

If your app or third-party SDK doesn’t connect, or no longer connects to any tracking domains, remove both `NSPrivacyTrackingDomains` and `NSPrivacyTracking` keys from your privacy manifest. Alternatively, set the value of `NSPrivacyTracking` to `false` and remove `NSPrivacyTrackingDomains` from your privacy manifest.

## Possible reasons for an invalid accessed API type value

The following table lists reasons why a value for the `NSPrivacyAccessedAPIType` key is invalid:

| Reason | Solution |
|----|----|
| The value is any other type than a string. | Change the type of the `NSPrivacyAccessedAPIType` key to `String` in your privacy manifest. |
| The value is an empty string, or a string whose value doesn’t match a category of required reason APIs. | Set the value of the `NSPrivacyAccessedAPIType` key to a string that exactly matches a category of required reason APIs your app uses. For possible values, see Describing use of required reason API. |

## Possible reasons for an invalid accessed API type reasons value

The following table lists reasons why a value for the `NSPrivacyAccessedAPITypeReasons` key is invalid:

| Reason | Solution |
|----|----|
| The value is any other type than an array of strings. | Change the type of the `NSPrivacyAccessedAPITypeReasons` key to `Array` in your privacy manifest. |
| The value is an empty array of strings. | In the dictionary that contains the `NSPrivacyAccessedAPITypeReasons` key, check the value of the `NSPrivacyAccessedAPIType` key. Add one or more reason strings to the array whose value exactly matches a value associated with `NSPrivacyAccessedAPIType`. |
| The value is an array of strings, but some entries don’t match the expected values for the `NSPrivacyAccessedAPIType` key you provide. | In the dictionary that contains the `NSPrivacyAccessedAPITypeReasons` key, check the value of the `NSPrivacyAccessedAPIType` key. Confirm each reason string in the array exactly matches a value associated with `NSPrivacyAccessedAPIType`. |

Note

If your app or third-party SDK doesn’t use, or no longer uses a specific required reason API, remove its related dictionary from the `NSPrivacyAccessedAPITypes` key. If `NSPrivacyAccessedAPITypes` is empty, remove it from the privacy manifest.

## Possible reasons for an invalid accessed API types value

The following table lists reasons why a value for the `NSPrivacyAccessedAPITypes` key is invalid:

| Reason | Solution |
|----|----|
| The value is any other type than an array of dictionaries. | Change the type of the `NSPrivacyAccessedAPITypes` key to `Array` in your privacy manifest. |
| The value is an empty array of dictionaries. | Create a dictionary that includes information about a required reason API your app or third-party SDK uses, then add the dictionary to the array. Repeat the process for all required reason APIs your app or third-party SDK uses. |
| The value is an array of dictionaries, but some of the dictionaries are invalid. | Confirm each dictionary in the array contains a `NSPrivacyAccessedAPIType` key and a `NSPrivacyAccessedAPITypeReasons` key, and both keys contain valid values. |

## Validate your privacy manifest file

You can use the `plutil` command to ensure your privacy manifest is a properly formatted plist file. To validate your privacy manifest, run `plutil` with the `-lint` option in Terminal:

```
```

If the privacy manifest is a valid plist, the command prints a message similar to the following:

```
```

If the privacy manifest is malformed, an error message appears in Terminal:

```
```

To fix the errors, open your privacy manifest in a text editor or Xcode to address them.

Note

If your privacy manifest is a valid plist, check its keys and values. Your privacy manifest could still be invalid if its keys and values don’t match the values App Store Connect expects. For more information about the keys and values App Store Connect expects, see Privacy manifest files.

## Revision History

- **2024-11-12** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

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

