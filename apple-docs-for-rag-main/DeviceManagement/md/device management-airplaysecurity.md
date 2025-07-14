

- Device Management
-  AirPlaySecurity 

Device Management Profile

# AirPlaySecurity

The payload you use to configure Apple TV for a particular style of AirPlay security.

tvOS 11.0+Device Assignment ServicesVPP License Management

``` source
object AirPlaySecurity
```

## Properties

`AccessType`

`string`

 (Required) 

The access policy for AirPlay.

`ANY` allows connections from both Ethernet/WiFi and Apple Wireless Direct Link.

`WIFI_ONLY` allows connections only from devices on the same Ethernet/WiFi network as Apple TV.

Possible Values: `ANY, WIFI_ONLY`

`Password`

`string`

The AirPlay password; required if `SecurityType` is `PASSWORD`.

`SecurityType`

`string`

 (Required) 

The security policy for AirPlay. Allowed values:

`PASSCODE_ONCE`  
Requires an onscreen passcode on first connection from a device. Subsequent connections from the same device aren’t prompted.

`PASSCODE_ALWAYS`  
Requires an onscreen passcode for every AirPlay connection. After an AirPlay connection ends, the system allows reconnecting within 30 seconds without a password.

`PASSWORD`  
Requires the passphrase set for `Password`.

Note

`NONE` was deprecated in tvOS 11.3. Existing profiles that use `NONE` get the `PASSWORD_ONCE` behavior.

Possible Values: `PASSCODE_ONCE, PASSCODE_ALWAYS, PASSWORD`

## Discussion

Specify `com.apple.airplay.security` as the payload type.

### Profile Availability

|                            |      |
|----------------------------|------|
| Device Channel             | tvOS |
| User Channel               | \-   |
| Allow Manual Install       | tvOS |
| Requires Supervision       | \-   |
| Requires User Approved MDM | \-   |
| Allowed in User Enrollment | \-   |
| Allow Multiple Payloads    | \-   |

### Profile Example

```

    PayloadContent

            Password
            MyPassword
            PayloadIdentifier
            com.example.myairplaysecuritypayload
            PayloadType
            com.apple.airplay.security
            PayloadUUID
            c0b60f19-91c7-482e-9a95-6ba71220d93e
            PayloadVersion
            1
            SecurityType
            PASSWORD
            AccessType
            ANY

    PayloadDisplayName
    AirPlay Security
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    40dc47ea-41c9-4c79-8b30-a027cf6eacd6
    PayloadVersion
    1

```

## See Also

### AirPlay

object AirPlay

The payload you use to configure AirPlay settings.

