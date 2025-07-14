

- User Notifications
- UNUserNotificationCenter
-  getDeliveredNotifications(completionHandler:) 

Instance Method

# getDeliveredNotifications(completionHandler:)

Fetches all of your app’s delivered notifications that are still present in Notification Center.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
func getDeliveredNotifications(completionHandler: @escaping ([UNNotification]) -> Void)
```

``` source
func deliveredNotifications() async -> [UNNotification]
```

## Parameters 

`completionHandler`  

The block to execute with the results. This block may be executed on a background thread. The block has no return value and takes the following parameter:

notifications  
An array of UNNotification objects representing the local and remote notifications of your app that have been delivered and are still visible in Notification Center. If none of your app’s notifications are visible in Notification Center, the array is empty.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func deliveredNotifications() async -> [UNNotification]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method executes asynchronously, returning immediately and executing the provided block on a background thread when the results become available.

## See Also

### Removing delivered notifications

func removeDeliveredNotifications(withIdentifiers: [String])

Removes your app’s notifications from Notification Center that match the specified identifiers.

func removeAllDeliveredNotifications()

Removes all of your app’s delivered notifications from Notification Center.

