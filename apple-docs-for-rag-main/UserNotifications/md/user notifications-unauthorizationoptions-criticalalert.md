

- User Notifications
- UNAuthorizationOptions
-  criticalAlert 

Type Property

# criticalAlert

The ability to play sounds for critical alerts.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static var criticalAlert: UNAuthorizationOptions { get }
```

## Discussion

Critical alerts ignore the mute switch and Do Not Disturb; the system plays a critical alert’s sound regardless of the device’s mute or Do Not Disturb settings. You can specify a custom sound and volume.

Critical alerts require a special entitlement issued by Apple.

## See Also

### Options

static var badge: UNAuthorizationOptions

The ability to update the app’s badge.

static var sound: UNAuthorizationOptions

The ability to play sounds.

static var alert: UNAuthorizationOptions

The ability to display alerts.

static var carPlay: UNAuthorizationOptions

The ability to display notifications in a CarPlay environment.

static var providesAppNotificationSettings: UNAuthorizationOptions

An option indicating the system should display a button for in-app notification settings.

static var provisional: UNAuthorizationOptions

The ability to post noninterrupting notifications provisionally to the Notification Center.

