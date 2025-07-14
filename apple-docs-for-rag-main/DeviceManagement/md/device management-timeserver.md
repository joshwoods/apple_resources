

- Device Management
-  TimeServer 

Device Management Profile

# TimeServer

The payload you use to configure the time server.

macOS 10.12.4+Device Assignment ServicesVPP License Management

``` source
object TimeServer
```

## Properties

`timeServer`

`string`

The NTP server to connect to. In macOS 10.13 and earlier, use commas to separate multiple time servers.

`timeZone`

`string`

The time zone path location string in `/usr/share/zoneinfo/`; for example, `America/Denver` or `Zulu`.

## Discussion

Specify `com.apple.MCX` as the payload type.

If multiple profiles with this payload are sent, the system sets the device’s time server to the value in the last payload installed. Removing the payload won’t change the settings back to the prior settings.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            timeServer
            ntp.example.com
            timeZone
            America/Denver
            PayloadIdentifier
            com.example.mytimeserverpayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            7bc24f5a-5ad8-4ad0-b05e-8f5f4418ff05
            PayloadVersion
            1

    PayloadDisplayName
    Time Server
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    a18b9fa3-dbdc-4e60-89e0-d785c7c6a1a0
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

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

