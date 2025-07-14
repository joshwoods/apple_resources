

- WatchKit
- WKUserNotificationInterfaceController
-  init() 

Initializer

# init()

Initializes and returns the interface controller using the specified remote notification data.

watchOS 2.0+

``` source
@MainActor
init()
```

## Return Value

The initialized interface controller.

## Discussion

Use this method to initialize your notification interface controller and prepare it for display. You must call the `super` implementation of this method first. That method creates the interface objects for the outlets declared in your class and referencing items in your storyboard.

At some point after initialization, WatchKit calls the `didReceiveRemoteNotification(_:withCompletion:)` or `didReceive(_:withCompletion:)` method to deliver the notification payload.

## See Also

### Related Documentation

App Programming Guide for watchOS

