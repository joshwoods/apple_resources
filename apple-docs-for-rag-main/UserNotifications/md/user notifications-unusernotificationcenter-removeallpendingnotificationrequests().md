

- User Notifications
- UNUserNotificationCenter
-  removeAllPendingNotificationRequests() 

Instance Method

# removeAllPendingNotificationRequests()

Removes all of your app’s pending local notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func removeAllPendingNotificationRequests()
```

## Discussion

This method executes asynchronously, removing all pending notification requests on a secondary thread.

```
let center = UNUserNotificationCenter.current()
center.removeAllPendingNotificationRequests()
```

## See Also

### Scheduling notifications

func add(UNNotificationRequest, withCompletionHandler: (((any Error)?) -> Void)?)

Schedules the delivery of a local notification.

func getPendingNotificationRequests(completionHandler: ([UNNotificationRequest]) -> Void)

Fetches all of your app’s local notifications that are pending delivery.

func removePendingNotificationRequests(withIdentifiers: [String])

Removes your app’s local notifications that are pending and match the specified identifiers.

