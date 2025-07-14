

- User Notifications
- UNUserNotificationCenter
-  getPendingNotificationRequests(completionHandler:) 

Instance Method

# getPendingNotificationRequests(completionHandler:)

Fetches all of your app’s local notifications that are pending delivery.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func getPendingNotificationRequests(completionHandler: @escaping ([UNNotificationRequest]) -> Void)
```

``` source
func pendingNotificationRequests() async -> [UNNotificationRequest]
```

## Parameters 

`completionHandler`  

A block for processing notification requests. This block may be executed on a background thread. The block has no return value and takes a single parameter.

requests  
An array of UNNotificationRequest objects representing the scheduled notification requests. If there are no scheduled requests, this array is empty.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func pendingNotificationRequests() async -> [UNNotificationRequest]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Here’s an example that obtains the pending notification requests.

```
let center = UNUserNotificationCenter.current()
let requests = await center.pendingNotificationRequests()
```

## See Also

### Scheduling notifications

func add(UNNotificationRequest, withCompletionHandler: (((any Error)?) -> Void)?)

Schedules the delivery of a local notification.

func removePendingNotificationRequests(withIdentifiers: [String])

Removes your app’s local notifications that are pending and match the specified identifiers.

func removeAllPendingNotificationRequests()

Removes all of your app’s pending local notifications.

