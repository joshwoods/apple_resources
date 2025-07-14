

- Device Management
-  ScreensaverUser 

Device Management Profile

# ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object ScreensaverUser
```

## Properties

`idleTime`

`integer`

The number of seconds of inactivity before the screen saver activates (`0` = Never activate).

`moduleName`

`string`

 (Required) 

The name of the screen saver module.

`modulePath`

`string`

A full path to the screen-saver module to use.

## Discussion

Specify `com.apple.screensaver.user` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | \-    |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            idleTime
            60
            modulePath
            /System/Library/Screen Savers/Name.saver
            PayloadIdentifier
            com.example.myscreensaverpayload
            PayloadType
            com.apple.screensaver.user
            PayloadUUID
            c5dceece-f633-44e6-b899-9d46631fd6e5
            PayloadVersion
            1

    PayloadDisplayName
    Screen Saver User
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    59332e00-d3c5-4d2a-a23a-ba36e45034e9
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

object SetupAssistant

The payload you use to configure setup-assistant settings.

object TimeMachine

The payload you use to configure Time Machine.

