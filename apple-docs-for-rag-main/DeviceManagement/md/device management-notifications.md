

- Device Management
-  Notifications 

Device Management Profile

# Notifications

The payload you use to configure notifications.

iOS 9.3+iPadOS 9.3+macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object Notifications
```

## Properties

`NotificationSettings`

`[`Notifications.NotificationSettingsItem`]`

 (Required) 

An array of notification settings dictionaries.

## Discussion

Specify `com.apple.notificationsettings` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | macOS, iOS              |
| Requires Supervision       | iOS                     |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | \-                      |
| Allow Multiple Payloads    | macOS                   |

### Profile Example

```

    PayloadContent

            NotificationSettings

                    AlertType
                    0
                    BundleIdentifier
                    com.apple.mobilemail
                    NotificationsEnabled

            ShowInLockScreen

            PayloadIdentifier
            com.example.mynotificationspayload
            PayloadType
            com.apple.notificationsettings
            PayloadUUID
            d1cc23d9-f482-40c5-b7b1-332149659986
            PayloadVersion
            1

    PayloadDisplayName
    Notification
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2bb0ab2e-1e0a-4c03-a662-b4ee2ffe224a
    PayloadVersion
    1

```

## Topics

### Objects

object Notifications.NotificationSettingsItem

The notification settings dictionary.

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

object ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

object SetupAssistant

The payload you use to configure setup-assistant settings.

object TimeMachine

The payload you use to configure Time Machine.

