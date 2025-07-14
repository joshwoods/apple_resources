

- User Notifications
- UNUserNotificationCenter
-  removePendingNotificationRequests(withIdentifiers:) 

Instance Method

# removePendingNotificationRequests(withIdentifiers:)

Removes your app’s local notifications that are pending and match the specified identifiers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func removePendingNotificationRequests(withIdentifiers identifiers: [String])
```

## Parameters 

`identifiers`  

An array of NSString objects, each of which contains the identifier of an active UNNotificationRequest object. If the identifier belongs to a non repeating request, and the trigger condition for that request has already been met, this method ignores the identifier.

## Discussion

This method executes asynchronously, removing the pending notification requests on a secondary thread.

```
let center = UNUserNotificationCenter.current()
center.removePendingNotificationRequests(withIdentifiers: ["com.example.mynotification"])
```

## See Also

### Scheduling notifications

func add(UNNotificationRequest, withCompletionHandler: (((any Error)?) -> Void)?)

Schedules the delivery of a local notification.

func getPendingNotificationRequests(completionHandler: ([UNNotificationRequest]) -> Void)

Fetches all of your app’s local notifications that are pending delivery.

func removeAllPendingNotificationRequests()

Removes all of your app’s pending local notifications.

