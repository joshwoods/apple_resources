

- Device Management
-  ProfileRemovalPassword 

Device Management Profile

# ProfileRemovalPassword

The payload you use to configure profile removal.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+Device Assignment ServicesVPP License Management

``` source
object ProfileRemovalPassword
```

## Properties

`RemovalPassword`

`string`

The password to allow removing the profile.

## Discussion

Specify `com.apple.profileRemovalPassword` as the payload type.

This payload provides a password to allow users to remove a locked configuration profile from the device. If this payload is present and has a password value set, the device asks for the password when the user taps a profile’s Remove button. This system encrypts the payload with the rest of the profile.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, macOS, tvOS |
| User Channel               | macOS            |
| Allow Manual Install       | iOS, macOS, tvOS |
| Requires Supervision       | iOS, tvOS        |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | \-               |
| Allow Multiple Payloads    | \-               |

### Profile Example

```

    PayloadContent

            RemovalPassword
            Password123
            PayloadIdentifier
            com.example.myprofileremovalpasswordprofile
            PayloadType
            com.apple.profileRemovalPassword
            PayloadUUID
            55f87465-a869-4ab0-9031-11ca1073641b
            PayloadVersion
            1

    PayloadDisplayName
    Password Removal
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    a42bfe59-7f3a-46a0-9908-4a5095fd2c6d
    PayloadVersion
    1
    HasRemovalPasscode

```

## See Also

### Managed Devices

object EducationConfiguration

The payload you use to configure the users, groups, and departments within an educational organization.

object LightsOutManagementLOM

The payload you use to configure lights-out management (LOM) settings.

object ManagedPreferences

The payload you use to configure managed preferences.

object MDM

The payload you use to configure mobile device management (MDM) settings.

