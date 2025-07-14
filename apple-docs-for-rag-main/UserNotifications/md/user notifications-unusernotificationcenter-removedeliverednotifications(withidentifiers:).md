

- User Notifications
- UNUserNotificationCenter
-  removeDeliveredNotifications(withIdentifiers:) 

Instance Method

# removeDeliveredNotifications(withIdentifiers:)

Removes your app’s notifications from Notification Center that match the specified identifiers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
func removeDeliveredNotifications(withIdentifiers identifiers: [String])
```

## Parameters 

`identifiers`  

An array of NSString objects, each of which corresponds to a value in the identifier property of a UNNotificationRequest object. This method ignores the identifiers of requests whose notifications are not currently displayed in Notification Center.

## Discussion

Use this method to selectively remove notifications that you no longer want displayed in Notification Center. The method executes asynchronously, returning immediately and removing the specified notifications on a background thread.

## See Also

### Removing delivered notifications

func getDeliveredNotifications(completionHandler: ([UNNotification]) -> Void)

Fetches all of your app’s delivered notifications that are still present in Notification Center.

func removeAllDeliveredNotifications()

Removes all of your app’s delivered notifications from Notification Center.

