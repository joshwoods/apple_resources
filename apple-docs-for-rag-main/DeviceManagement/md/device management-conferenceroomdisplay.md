

- Device Management
-  ConferenceRoomDisplay 

Device Management Profile

# ConferenceRoomDisplay

The payload you use to configure Conference Room Display mode for Apple TV.

tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object ConferenceRoomDisplay
```

## Properties

`Message`

`string`

The custom message displayed on the screen in Conference Room Display mode.

## Discussion

Specify `com.apple.conferenceroomdisplay` as the payload type.

Conference Room Display mode locks Apple TV into that mode, to prevent other types of usage.

### Profile Availability

|                            |      |
|----------------------------|------|
| Device Channel             | tvOS |
| User Channel               | \-   |
| Allow Manual Install       | tvOS |
| Requires Supervision       | tvOS |
| Requires User Approved MDM | \-   |
| Allowed in User Enrollment | \-   |
| Allow Multiple Payloads    | \-   |

### Profile Example

```

    PayloadContent

            Message
            Display Message
            PayloadIdentifier
            com.example.myconferenceroompayload
            PayloadType
            com.apple.conferenceroomdisplay
            PayloadUUID
            2aff0bfa-62f4-4597-9714-3750f5e3d422
            PayloadVersion
            1

    PayloadDisplayName
    Conference Room Display
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    c98885c9-12fe-43d2-8476-fb98bc959dd3
    PayloadVersion
    1

```

## See Also

### Apple TV

object TVRemote

The payload you use to configure the Apple TV remote.

