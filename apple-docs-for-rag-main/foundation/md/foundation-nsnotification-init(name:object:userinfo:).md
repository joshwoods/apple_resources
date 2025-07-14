

- Foundation
- NSNotification
-  init(name:object:userInfo:) 

Initializer

# init(name:object:userInfo:)

Initializes a notification with a specified name, object, and user information.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    name: NSNotification.Name,
    object: Any?,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`name`  

The name for the new notification. May not be `nil`.

`object`  

The object for the new notification.

`userInfo`  

The user information dictionary for the new notification. May be `nil`.

## See Also

### Creating Notifications

init?(coder: NSCoder)

Initializes a notification with the data from an unarchiver.

convenience init(name: NSNotification.Name, object: Any?)

Returns a new notification object with a specified name and object.

struct Name

A structure that defines the name of a notification.

