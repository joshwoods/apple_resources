

- Device Management
-  ParentalControlsTimeLimits 

Device Management Profile

# ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsTimeLimits
```

## Properties

`familyControlsEnabled`

`boolean`

 (Required) 

If `true`, enables time limits.

`time-limits`

ParentalControlsTimeLimits.Time-limits

The time limits to enforce if `familyControlsEnabled` is enabled.

## Discussion

Specify `com.apple.familycontrols.timelimits.v2` as the payload type.

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

            familyControlsEnabled

            limits-list

                    allowancesActive

                    groupID
                    __COMPUTER__
                    itemType
                    com.apple.familycontrols.timelimits.computer
                    name
                    Computer
                    allowances

                            fromDay
                            0
                            span
                            0
                            toDay
                            4
                            timeLimitSeconds
                            1800

                            fromDay
                            5
                            span
                            0
                            toDay
                            6
                            timeLimitSeconds
                            1800

            PayloadIdentifier
            com.example.mytimelimitspayload
            PayloadType
            com.apple.familycontrols.timelimits.v2
            PayloadUUID
            0b17c132-352d-4a3a-9f76-b016f7f0ad6c
            PayloadVersion
            1

    PayloadDisplayName
    Parental Controls Time Limits
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    5c7a4e4b-1a9e-4586-9f31-b04e818a84b2
    PayloadVersion
    1

```

## Topics

### Objects

object ParentalControlsTimeLimits.Time-limits

The time limits dictionary.

## See Also

### Parental Controls

object ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

object ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

object ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

object ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

