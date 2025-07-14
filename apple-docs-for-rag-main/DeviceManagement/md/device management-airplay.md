

- Device Management
-  AirPlay 

Device Management Profile

# AirPlay

The payload you use to configure AirPlay settings.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object AirPlay
```

## Properties

`AllowList`

`[`AirPlay.AllowListItem`]`

If present, only AirPlay destinations in this list are available to the device. This allow list applies to supervised devices.

`Passwords`

`[`AirPlay.PasswordsItem`]`

If present, sets passwords for known AirPlay destinations. Using multiple entries for the same destination, whether within the same payload or across multiple installed payloads, is an error and results in undefined behavior.

`Whitelist`

`[`AirPlay.AllowListItem`]`

Deprecated 

Use `AllowList` instead. This key is deprecated in iOS 14.5 and macOS 11.3.

## Discussion

Specify `com.apple.airplay` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS                   |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS, macOS              |
| Allow Multiple Payloads    | iOS, macOS              |

### Profile Example

```

    PayloadContent

            Passwords

                    DeviceName
                    Juan&apos;s Apple TV
                    Password
                    Password123

            Whitelist

                    DeviceID
                    64:C7:53:EB:DB:B4

            PayloadIdentifier
            com.example.myairplaysettingspayload
            PayloadType
            com.apple.airplay
            PayloadUUID
            dfb67669-67eb-4ed4-ad4f-1f8861029b42
            PayloadVersion
            1

    PayloadDisplayName
    AirPlay
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    c6ec425e-b224-45fb-8889-7475cb3814cb
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object AirPlay.AllowListItem

The dictionary that defines allowed destinations.

object AirPlay.PasswordsItem

The dictionary that defines passwords for AirPlay destinations.

## See Also

### AirPlay

object AirPlaySecurity

The payload you use to configure Apple TV for a particular style of AirPlay security.

