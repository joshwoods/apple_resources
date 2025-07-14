

- UIKit
-  UIUserNotificationType Deprecated

Structure

# UIUserNotificationType

Constants indicating how the app alerts the user when a local or push notification arrives.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
struct UIUserNotificationType
```

## Topics

### Constants

static var badge: UIUserNotificationType

The app badges its icon.

static var sound: UIUserNotificationType

The app plays a sound.

static var alert: UIUserNotificationType

The app posts an alert.

### Initializers

init(rawValue: UInt)

Creates a notification type with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

