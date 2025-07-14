

- Device Management
-  Font 

Device Management Profile

# Font

The payload you use to configure fonts.

iOS 7.0+iPadOS 7.0+macOS 10.9+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object Font
```

## Properties

`Font`

`data`

 (Required) 

The contents of the font file.

`Name`

`string`

The user-visible name for the font. This field is replaced by the actual name of the font after installation. Each payload must contain exactly one font file in trueType (.ttf) or OpenType (.otf) format. Collection formats (.ttc or .otc) are not supported.

Fonts are identified by their embedded PostScript names. Two fonts with the same PostScript name are considered to be the same font even if their contents differ. Installing two different fonts with the same PostScript name isn’t supported, and the resulting behavior is undefined.

Default:

## Discussion

Specify `com.apple.font` as the payload type.

In iPadOS 18 and later, the font profile is available on the user channel for shared iPads.

### Profile Availability

|                            |                    |
|----------------------------|--------------------|
| Device Channel             | iOS, macOS         |
| User Channel               | macOS, Shared iPad |
| Allow Manual Install       | iOS, macOS         |
| Requires Supervision       | \-                 |
| Requires User Approved MDM | \-                 |
| Allowed in User Enrollment | iOS, macOS         |
| Allow Multiple Payloads    | iOS, macOS         |

### Profile Example

```

    PayloadContent

            Font
            base64encodeddata
            Name
            Font.ttf
            PayloadIdentifier
            com.example.myfontpayload
            PayloadType
            com.apple.font
            PayloadUUID
            99659c06-bbbf-45aa-9674-06b378ec2cd5
            PayloadVersion
            1

    PayloadDisplayName
    Fonts
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    9800ea91-30c4-4212-8033-d21cad4fe99a
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

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

