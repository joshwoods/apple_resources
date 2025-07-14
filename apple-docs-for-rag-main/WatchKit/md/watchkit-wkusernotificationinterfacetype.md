

- WatchKit
-  WKUserNotificationInterfaceType 

Enumeration

# WKUserNotificationInterfaceType

The type of notification interface to display.

watchOS

``` source
enum WKUserNotificationInterfaceType
```

## Topics

### Constants

case `default`

A constant indicating that the system should display the corresponding static interface instead. When you return this value, the system takes responsibility for displaying the notification’s content.

case custom

A constant indicating that the system should display your dynamic notification interface.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

