

- Device Management
-  LockScreenMessage 

Device Management Profile

# LockScreenMessage

The payload you use to configure a Lock screen message.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object LockScreenMessage
```

## Properties

`AssetTagInformation`

`string`

The asset tag information for the device, displayed in the login window and Lock screen.

`IfLostReturnToMessage`

`string`

Deprecated 

Deprecated. Use `LockScreenFootnote` instead.

`LockScreenFootnote`

`string`

The footnote displayed in the login window and Lock screen.

## Discussion

Specify `com.apple.shareddeviceconfiguration` as the payload type.

This payload allows administrators to specify optional text displayed in the login window and Lock screen (for example, an “If Lost, Return To” message and asset tag information). There can only be one Lock screen payload.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Allow Manual Install       | iOS              |
| Requires Supervision       | iOS              |
| Requires User-Approved MDM | \-               |
| Allowed in User Enrollment | \-               |
| Allow Multiple Payloads    | \-               |

### Profile Example

```

    PayloadContent

            AssetTagInformation
            1234
            IfLostReturnToMessage
            Example message
            PayloadIdentifier
            com.example.mylockscreenpayload
            PayloadType
            com.apple.shareddeviceconfiguration
            PayloadUUID
            b10c0436-a51b-4119-b604-bd580f396723
            PayloadVersion
            1

    PayloadDisplayName
    Lock Screen Message
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    588f1406-47be-47fc-9907-4e7955fb6d4a
    PayloadVersion
    1

```

## See Also

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object EnergySaver

The payload you use to configure energy-saver settings.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

