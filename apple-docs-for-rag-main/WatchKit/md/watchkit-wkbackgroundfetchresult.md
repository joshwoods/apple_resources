

- WatchKit
-  WKBackgroundFetchResult 

Enumeration

# WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

watchOS 6.0+

``` source
enum WKBackgroundFetchResult
```

## Topics

### Fetch Results

case failed

The download attempt failed.

case newData

The download attempt succeeded.

case noData

The notification has no associated content.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing remote notifications

func didRegisterForRemoteNotifications(withDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func didFailToRegisterForRemoteNotificationsWithError(any Error)

Tells the delegate that Apple Push Notification service (APNs) can’t successfully complete the registration process.

func didReceiveRemoteNotification([AnyHashable : Any], fetchCompletionHandler: (WKBackgroundFetchResult) -> Void)

Tells the delegate that a background notification has arrived.

