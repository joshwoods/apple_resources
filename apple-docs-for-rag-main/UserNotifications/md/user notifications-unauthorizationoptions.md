

- User Notifications
-  UNAuthorizationOptions 

Structure

# UNAuthorizationOptions

Options that determine the authorized features of local and remote notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct UNAuthorizationOptions
```

## Topics

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

static var providesAppNotificationSettings: UNAuthorizationOptions

An option indicating the system should display a button for in-app notification settings.

static var provisional: UNAuthorizationOptions

The ability to post noninterrupting notifications provisionally to the Notification Center.

### Initializers

init(rawValue: UInt)

Initializes an authorization options constant using the specified raw value.

### Deprecated

static var announcement: UNAuthorizationOptions

The ability for Siri to automatically read out messages over AirPods.

Deprecated

static var timeSensitive: UNAuthorizationOptionsDeprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Requesting authorization

func requestAuthorization(options: UNAuthorizationOptions, completionHandler: (Bool, (any Error)?) -> Void)

Requests a person’s authorization to allow local and remote notifications for your app.

