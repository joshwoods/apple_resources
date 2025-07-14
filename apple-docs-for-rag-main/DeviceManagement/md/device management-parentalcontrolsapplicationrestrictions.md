

- Device Management
-  ParentalControlsApplicationRestrictions 

Device Management Profile

# ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsApplicationRestrictions
```

## Properties

`familyControlsEnabled`

`boolean`

 (Required) 

If `true`, enables app access restrictions.

`pathBlackList`

`[string]`

Deprecated 

The paths to apps in the deny list. This property is deprecated in macOS 10.15 and later.

`pathWhiteList`

`[string]`

Deprecated 

The paths to apps in the allow list. This property is deprecated in macOS 10.15 and later.

`whiteList`

`[`ParentalControlsApplicationRestrictions.ApplicationItem`]`

The allow list of app item dictionaries.

## Discussion

Specify `com.apple.applicationaccess.new` as the payload type.

To determine if an app can be launched, the app is evaluated with these rules:

- Certain system app and utilities are always allowed to run.

- The allow list is searched to see if the `bundleID` has a matching entry. If a match is found, `appID` and `detachedSignature` (if present) are used to verify the signature of the app being launched. If the signature is valid and matches the designated requirement (in the appID key), the app is allowed to launch.

- If the path to the binary being launched matches or is in a subdirectory of a path in the deny list, the binary is denied.

- If the path to the binary being launched matches or is a subdirectory of a path in the allow list, the binary is allowed to launch.

- The binary is denied permission to launch.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            familyControlsEnabled

            pathBlackList

                /Applications/Utilities

            pathWhiteList

                /Applications/Utilities

            whiteList

                    appID
                    +t4MAAAAADAAAAABAAAABgAAAAIAAAASY29tLmFwcGxlLlRleHRFZGl0AAAAAAAD
                    appStore

                    bundleID
                    com.example.myotherapp
                    displayName
                    My App
                    subApps

            PayloadIdentifier
            com.example.myapplicationrestrictionspayload
            PayloadType
            com.apple.applicationaccess.new
            PayloadUUID
            e5af83ab-e936-495a-b6b7-05b113cf530e
            PayloadVersion
            1

    PayloadDisplayName
    Parental Controls Application Restrictions
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    144fbebc-4db4-4642-83eb-78eed2992578
    PayloadVersion
    1

```

## Topics

### Objects

object ParentalControlsApplicationRestrictions.ApplicationItem

A dictionary defining an app for parental control.

## See Also

### Parental Controls

object ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

object ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

object ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

object ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

