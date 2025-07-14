

- Foundation
- Notification
-  init(name:object:userInfo:) 

Initializer

# init(name:object:userInfo:)

Initializes a new notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    name: Notification.Name,
    object: Any? = nil,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Discussion

The default value for `userInfo` is nil.

## See Also

### Creating a Notification

typealias Name

An alias for a type used to represent the name of a notification.

struct Name

A structure that defines the name of a notification.

