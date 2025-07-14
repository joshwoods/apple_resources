

- User Notifications
-  UNNotificationActionOptions 

Structure

# UNNotificationActionOptions

The behaviors you can apply to an action.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
struct UNNotificationActionOptions
```

## Topics

### Initializers

init(rawValue: UInt)

Initializes an action options object using the specified raw value.

### Constants

static var authenticationRequired: UNNotificationActionOptions

The action can be performed only on an unlocked device.

static var destructive: UNNotificationActionOptions

The action performs a destructive task.

static var foreground: UNNotificationActionOptions

The action causes the app to launch in the foreground.

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

### Getting Options

var options: UNNotificationActionOptions

The behaviors associated with the action.

