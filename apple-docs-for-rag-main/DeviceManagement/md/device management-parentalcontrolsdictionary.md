

- Device Management
-  ParentalControlsDictionary 

Device Management Profile

# ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsDictionary
```

## Properties

`parentalControl`

`boolean`

 (Required) 

If `true`, enables parental controls dictionary restrictions.

## Discussion

Specify `com.apple.Dictionary` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            parentalControl

            PayloadIdentifier
            com.example.mydictionarypayload
            PayloadType
            com.apple.Dictionary
            PayloadUUID
            0158853b-e3d5-41d6-b4d2-ada868a36042
            PayloadVersion
            1

    PayloadDisplayName
    Parental Controls Dictionary
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    9b0ea70d-b1b1-4a96-81e7-3b33bfd563d5
    PayloadVersion
    1

```

## See Also

### Parental Controls

object ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

object ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

object ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

object ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

