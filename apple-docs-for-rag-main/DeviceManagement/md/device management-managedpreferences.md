

- Device Management
-  ManagedPreferences 

Device Management Profile

# ManagedPreferences

The payload you use to configure managed preferences.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ManagedPreferences
```

## Properties

`PayloadContent`

ManagedPreferences.PayloadContent

 (Required) 

## Discussion

Specify `com.apple.ManagedClient.preferences` as the payload type.

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

            PayloadContent

                com.example.myapp

                    Forced

                            mcx_preference_settings

                                MySetting

            PayloadIdentifier
            com.example.mymanprefpayload
            PayloadType
            com.apple.ManagedClient.preferences
            PayloadUUID
            83c9f6e8-ef4b-4974-b83b-b2e7fe79b75c
            PayloadVersion
            1

    PayloadDisplayName
    Managed Preference
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    54e23577-3424-4092-a9b4-a5e5af88fd52
    PayloadVersion
    1

```

## Topics

### Profiles

object ManagedPreferences.PayloadContent

## See Also

### Managed Devices

object EducationConfiguration

The payload you use to configure the users, groups, and departments within an educational organization.

object LightsOutManagementLOM

The payload you use to configure lights-out management (LOM) settings.

object MDM

The payload you use to configure mobile device management (MDM) settings.

object ProfileRemovalPassword

The payload you use to configure profile removal.

