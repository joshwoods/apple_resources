

- Foundation
- NSNotification
-  init(coder:) 

Initializer

# init(coder:)

Initializes a notification with the data from an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(coder: NSCoder)
```

## See Also

### Creating Notifications

convenience init(name: NSNotification.Name, object: Any?)

Returns a new notification object with a specified name and object.

init(name: NSNotification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Initializes a notification with a specified name, object, and user information.

struct Name

A structure that defines the name of a notification.

