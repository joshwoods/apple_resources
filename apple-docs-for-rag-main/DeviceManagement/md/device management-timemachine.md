

- Device Management
-  TimeMachine 

Device Management Profile

# TimeMachine

The payload you use to configure Time Machine.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object TimeMachine
```

## Properties

`AutoBackup`

`boolean`

If `true`, performs automatic backups at regular intervals.

Default: `true`

`BackupAllVolumes`

`boolean`

If `true`, backs up only the startup volume by default.

Default: `false`

`BackupDestURL`

`string`

 (Required) 

The URL of the backup destination.

`BackupSizeMB`

`integer`

The backup size limit, in megabytes. Set to 0 for unlimited.

Default: `0`

`BackupSkipSys`

`boolean`

If `true`, skips system files and folders by default.

Default: `false`

`BasePaths`

`[string]`

The list of paths to back up besides the startup volume.

`MobileBackups`

`boolean`

If `true`, create local backup snapshots when not connected to the network.

Default: `true`

`SkipPaths`

`[string]`

The path to skip from start volume.

## Discussion

Specify `com.apple.MCX.TimeMachine` as the payload type.

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

            AutoBackup

            BackupAllVolumes

            BackupDestURL
            server.example.com
            BackupSizeMB
            1000
            BackupSkipSys

            MobileBackups

            SkipPaths

                /Users/Shared

            PayloadIdentifier
            com.example.mytimemachinepayload
            PayloadType
            com.apple.MCX.TimeMachine
            PayloadUUID
            5f0be3a6-c9b8-44db-a2ae-414311772fdb
            PayloadVersion
            1

    PayloadDisplayName
    Time Machine
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    68ca5f6c-13e8-43c3-b2ee-8bc405f5eed5
    PayloadVersion
    1

```

## See Also

### User Experience

object Accessibility

The payload you use to configure the accessibility features of the device.

object Desktop

The payload you use to configure the desktop.

object Dock

The payload you use to configure the dock.

object Finder

The payload you use to configure Finder settings.

object HomeScreenLayout

The payload you use to configure the Home screen layout.

object ManagedMenuExtras

The payload you use to configure menu extras.

object Notifications

The payload you use to configure notifications.

object ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

object SetupAssistant

The payload you use to configure setup-assistant settings.

