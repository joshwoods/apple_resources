

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  shouldSendContentAvailable 

Instance Property

# shouldSendContentAvailable

A Boolean value that indicates whether the push notification includes the content available flag.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
var shouldSendContentAvailable: Bool { get set }
```

## Discussion

When this property is true, the server includes the `content-available` flag in the push notification’s payload. That flag causes the system to wake or launch an app that isn’t currently running. The app then receives background execution time to download any data for the push notification, such as the set of changed records. If the app is already running in the foreground, the inclusion of this flag has no additional effect and the system delivers the notification to the app delegate for processing as usual.

The default value of this property is false.

## See Also

### Accessing the Notification Info

var shouldSendMutableContent: Bool

A Boolean value that indicates whether the push notification sets the mutable content flag.

