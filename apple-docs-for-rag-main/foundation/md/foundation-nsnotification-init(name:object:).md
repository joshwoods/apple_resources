

- Foundation
- NSNotification
-  init(name:object:) 

Initializer

# init(name:object:)

Returns a new notification object with a specified name and object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    name aName: NSNotification.Name,
    object anObject: Any?
)
```

## Parameters 

`aName`  

The name for the new notification. May not be `nil`.

`anObject`  

The object for the new notification.

## See Also

### Related Documentation

func post(name: NSNotification.Name, object: Any?)

Creates a notification with a given name and sender and posts it to the notification center.

Notification Programming Topics

### Creating Notifications

init?(coder: NSCoder)

Initializes a notification with the data from an unarchiver.

init(name: NSNotification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Initializes a notification with a specified name, object, and user information.

struct Name

A structure that defines the name of a notification.

