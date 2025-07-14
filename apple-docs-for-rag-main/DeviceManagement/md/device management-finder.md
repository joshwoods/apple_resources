

- Device Management
-  Finder 

Device Management Profile

# Finder

The payload you use to configure Finder settings.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Finder
```

## Properties

`ProhibitBurn`

`boolean`

If `true`, the system disables the Finder’s burn support.

Default: `false`

`ProhibitConnectTo`

`boolean`

If `true`, the system disables Connect to Server.

Default: `false`

`ProhibitEject`

`boolean`

If `true`, the system disables Eject.

Default: `false`

`ProhibitGoToFolder`

`boolean`

If `true`, the system disables Go to Folder.

Default: `false`

`ShowExternalHardDrivesOnDesktop`

`boolean`

If `false`, the system doesn’t show external hard drives on the Desktop.

Default: `true`

`ShowHardDrivesOnDesktop`

`boolean`

If `false`, the system doesn’t show internal hard drives on the Desktop.

Default: `false`

`ShowMountedServersOnDesktop`

`boolean`

If `false`, the system doesn’t show mounted file servers on the Desktop.

Default: `false`

`ShowRemovableMediaOnDesktop`

`boolean`

If `false`, the system doesn’t show removable media items on the Desktop.

Default: `true`

`WarnOnEmptyTrash`

`boolean`

If `false`, the system doesn’t warn the user before emptying the trash.

Default: `true`

`InterfaceLevel`

`string`

Deprecated 

Specifies whether Finder should operate in Simple or Full mode.

Possible Values: `Simple, Full`

## Discussion

Specify `com.apple.finder` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            InterfaceLevel
            Full
            ShowHardDrivesOnDesktop

            ShowExternalHardDrivesOnDesktop

            ShowRemovableMediaOnDesktop

            ShowMountedServersOnDesktop

            WarnOnEmptyTrash

            ProhibitConnectTo

            ProhibitEject

            ProhibitBurn

            ProhibitGoToFolder

            PayloadIdentifier
            com.example.myfinderpayload
            PayloadType
            com.apple.finder
            PayloadUUID
            feea617a-c8f2-4dce-afae-20b2fe5f9c9b
            PayloadVersion
            1

    PayloadDisplayName
    Finder
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2527bd12-fbc4-4957-a9e7-4afeb64e0246
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

object TimeMachine

The payload you use to configure Time Machine.

