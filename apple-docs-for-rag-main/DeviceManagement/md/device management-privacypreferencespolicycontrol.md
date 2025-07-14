

- Device Management
-  PrivacyPreferencesPolicyControl 

Device Management Profile

# PrivacyPreferencesPolicyControl

The payload you use to configure privacy preferences.

macOS 10.14+Device Assignment ServicesVPP License Management

``` source
object PrivacyPreferencesPolicyControl
```

## Properties

`Services`

PrivacyPreferencesPolicyControl.Services

 (Required) 

A dictionary whose keys are limited to the privacy policy control services. In the case of conflicting specifications, the most restrictive setting (deny) is used.

## Discussion

Specify `com.apple.TCC.configuration-profile-policy` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | \-    |
| Requires Supervision       | \-    |
| Requires User Approved MDM | macOS |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            Services

                PostEvent

                        Allowed

                        CodeRequirement
                        identifier com.apple.screensharing.agent
                        Comment
                        Allow PostEvent control for ScreensharingAgent
                        Identifier
                        com.apple.screensharing.agent
                        IdentifierType
                        bundleID

            PayloadIdentifier
            com.example.mytccpayload
            PayloadType
            com.apple.TCC.configuration-profile-policy
            PayloadUUID
            5AAF51E3-D21F-4CE6-B0AA-074D75916F68
            PayloadVersion
            1

    PayloadDisplayName
    Privacy Preferences Policy Control
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    221000F0-D07A-11E8-811E-D0817ADA38E4
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object PrivacyPreferencesPolicyControl.Services

The privacy policy control services dictionary that controls access on a per app basis.

