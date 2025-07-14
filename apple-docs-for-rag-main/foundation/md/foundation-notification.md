

- Foundation
-  Notification 

Structure

# Notification

A container for information broadcast through a notification center to all registered observers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Notification
```

## Topics

### Creating a Notification

init(name: Notification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Initializes a new notification.

typealias Name

An alias for a type used to represent the name of a notification.

struct Name

A structure that defines the name of a notification.

### Getting Notification Information

var name: Notification.Name

A tag identifying the notification.

var object: Any?

An object that the poster wishes to send to observers.

var userInfo: [AnyHashable : Any]?

Storage for values or objects related to this notification.

### Using Reference Types

class NSNotification

A container for information broadcast through a notification center to all registered observers.

### Operators

static func == (Notification, Notification) -> Bool

Compare two notifications for equality.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- ReferenceConvertible

## See Also

### Notifications

class NotificationCenter

A notification dispatch mechanism that enables the broadcast of information to registered observers.

class NotificationQueue

A notification center buffer.

