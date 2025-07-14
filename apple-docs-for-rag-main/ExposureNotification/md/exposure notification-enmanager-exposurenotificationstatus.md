

- Exposure Notification
- ENManager
-  exposureNotificationStatus 

Instance Property

# exposureNotificationStatus

A property that indicates the status of exposure notifications.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var exposureNotificationStatus: ENStatus { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

You can use key value observing to monitor for changes. The value of this property will be ENStatus.unknown until activate(completionHandler:) completes successfully.

This status can be affected by the user disabling exposure notifications, disabling bluetooth, or restricting the feature through parental controls.

## See Also

### Configuring the Manager

var exposureNotificationEnabled: Bool

A property that indicates that a user enabled exposure notification.

class var authorizationStatus: ENAuthorizationStatus

A property that reports the current authorization status of the app, and never prompts the user.

var dispatchQueue: dispatch_queue_t

The dispatch queue on which to invoke handlers.

