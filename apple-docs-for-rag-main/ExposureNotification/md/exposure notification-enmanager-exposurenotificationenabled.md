

- Exposure Notification
- ENManager
-  exposureNotificationEnabled 

Instance Property

# exposureNotificationEnabled

A property that indicates that a user enabled exposure notification.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var exposureNotificationEnabled: Bool { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

You can use key value observing to monitor for changes. The value of this property will be `NO` until activate(completionHandler:) completes successfully.

Note that even if the user enables exposure notifications, they may be inactive for other reasons, such as if the user turns off Bluetooth service. The exposureNotificationStatus property can be monitored for the status of exposure notifications.

## See Also

### Configuring the Manager

var exposureNotificationStatus: ENStatus

A property that indicates the status of exposure notifications.

class var authorizationStatus: ENAuthorizationStatus

A property that reports the current authorization status of the app, and never prompts the user.

var dispatchQueue: dispatch_queue_t

The dispatch queue on which to invoke handlers.

