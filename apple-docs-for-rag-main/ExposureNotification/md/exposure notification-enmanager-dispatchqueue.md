

- Exposure Notification
- ENManager
-  dispatchQueue 

Instance Property

# dispatchQueue

The dispatch queue on which to invoke handlers.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var dispatchQueue: dispatch_queue_t { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

The default is the main queue.

## See Also

### Configuring the Manager

var exposureNotificationStatus: ENStatus

A property that indicates the status of exposure notifications.

var exposureNotificationEnabled: Bool

A property that indicates that a user enabled exposure notification.

class var authorizationStatus: ENAuthorizationStatus

A property that reports the current authorization status of the app, and never prompts the user.

