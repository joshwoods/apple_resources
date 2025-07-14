

- User Notifications
-  UNNotificationPresentationOptions 

Structure

# UNNotificationPresentationOptions

Constants indicating how to present a notification in a foreground app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct UNNotificationPresentationOptions
```

## Topics

### Constants

static var badge: UNNotificationPresentationOptions

Apply the notification’s badge value to the app’s icon.

static var banner: UNNotificationPresentationOptions

Present the notification as a banner.

static var list: UNNotificationPresentationOptions

Show the notification in Notification Center.

static var sound: UNNotificationPresentationOptions

Play the sound associated with the notification.

static var alert: UNNotificationPresentationOptions

Display the alert using the content provided by the notification.

Deprecated

### Initializers

init(rawValue: UInt)

Initializes a notification presentation options object using the specified raw value.

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

### Receiving Notifications

func userNotificationCenter(UNUserNotificationCenter, willPresent: UNNotification, withCompletionHandler: (UNNotificationPresentationOptions) -> Void)

Asks the delegate how to handle a notification that arrived while the app was running in the foreground.

