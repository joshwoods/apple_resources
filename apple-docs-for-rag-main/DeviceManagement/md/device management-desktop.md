

- Device Management
-  Desktop 

Device Management Profile

# Desktop

The payload you use to configure the desktop.

macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object Desktop
```

## Properties

`locked`

`boolean`

Deprecated 

If `true`, locks the desktop picture. Replaced with allowWallpaperModification in macOS 10.13.

Default: `false`

`override-picture-path`

`string`

The path to the desktop picture. If set, this picture is always locked.

## Discussion

Specify `com.apple.desktop` as the payload type.

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

            locked

            override-picture-path
            ~/Desktop/background.png
            PayloadIdentifier
            com.example.mydesktoppayload
            PayloadType
            com.apple.desktop
            PayloadUUID
            77a7ad50-9e32-4afb-8aee-79ae0c392848
            PayloadVersion
            1

    PayloadDisplayName
    Desktop
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2e00699a-8e37-417d-94b2-97b85ff722a2
    PayloadVersion
    1

```

## See Also

### User Experience

object Accessibility

The payload you use to configure the accessibility features of the device.

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

object TimeMachine

The payload you use to configure Time Machine.

