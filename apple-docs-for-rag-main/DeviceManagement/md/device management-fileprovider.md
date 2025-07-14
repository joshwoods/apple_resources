

- Device Management
-  FileProvider 

Device Management Profile

# FileProvider

The payload you use to configure file provider settings.

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object FileProvider
```

## Properties

`AllowManagedFileProvidersToRequestAttribution`

`boolean`

If `true`, enables file providers access to the path of the requesting process.

Default: `false`

`ManagementAllowsKnownFolderSyncing`

`boolean`

Default: `true`

`ManagementKnownFolderSyncingAllowList`

`[string]`

## Discussion

Specify `com.apple.fileproviderd` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User-Approved MDM | macOS |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            AllowManagedFileProvidersToRequestAttribution

            PayloadIdentifier
            com.example.myfileproviderpayload
            PayloadType
            com.apple.fileproviderd
            PayloadUUID
            3ffb5741-f0f1-4fc2-9566-679ca8b10db1
            PayloadVersion
            1

    PayloadDisplayName
    FileProvider
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8efec75c-f1d3-4aaa-a4ef-104dc25cfc3d
    PayloadVersion
    1

```

## See Also

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object EnergySaver

The payload you use to configure energy-saver settings.

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

object TimeServer

The payload you use to configure the time server.

