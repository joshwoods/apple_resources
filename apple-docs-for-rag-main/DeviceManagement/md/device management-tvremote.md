

- Device Management
-  TVRemote 

Device Management Profile

# TVRemote

The payload you use to configure the Apple TV remote.

iOS 11.3+iPadOS 11.3+tvOS 11.3+Device Assignment ServicesVPP License Management

``` source
object TVRemote
```

## Properties

`AllowedRemotes`

`[`TVRemote.AllowedRemotesItem`]`

The array of valid devices that Apple TV can connect to.

`AllowedTVs`

`[`TVRemote.AllowedTVsItem`]`

The array of valid Apple TV identifiers that the remote can connect to.

## Discussion

Specify `com.apple.tvremote` as the payload type.

### Profile Availability

|                            |                        |
|----------------------------|------------------------|
| Device Channel             | iOS, Shared iPad, tvOS |
| User Channel               | Shared iPad            |
| Allow Manual Install       | iOS, tvOS              |
| Requires Supervision       | iOS, tvOS              |
| Requires User Approved MDM | \-                     |
| Allowed in User Enrollment | \-                     |
| Allow Multiple Payloads    | \-                     |

### Profile Example

```

    PayloadContent

            AllowedRemotes

                    RemoteDeviceID
                    10:10:10:10:10:10

            AllowedTVs

            PayloadIdentifier
            com.example.mytvremotepayload
            PayloadType
            com.apple.tvremote
            PayloadUUID
            696eb2c4-df9d-463f-b74a-685dae845fac
            PayloadVersion
            1

    PayloadDisplayName
    TV Remote
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    3de47695-ad92-44f5-9bc9-f1b2f2c7727b
    PayloadVersion
    1

```

## Topics

### Objects

object TVRemote.AllowedRemotesItem

The array of valid devices that Apple TV can connect to.

object TVRemote.AllowedTVsItem

The array of valid Apple TV identifiers that the remote can connect to.

## See Also

### Apple TV

object ConferenceRoomDisplay

The payload you use to configure Conference Room Display mode for Apple TV.

