

- User Notifications
- UNAuthorizationOptions
-  providesAppNotificationSettings 

Type Property

# providesAppNotificationSettings

An option indicating the system should display a button for in-app notification settings.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static var providesAppNotificationSettings: UNAuthorizationOptions { get }
```

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

static var criticalAlert: UNAuthorizationOptions

The ability to play sounds for critical alerts.

static var provisional: UNAuthorizationOptions

The ability to post noninterrupting notifications provisionally to the Notification Center.

