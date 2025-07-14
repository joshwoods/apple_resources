

- User Notifications
- UNUserNotificationCenter
-  add(\_:withCompletionHandler:) 

Instance Method

# add(\_:withCompletionHandler:)

Schedules the delivery of a local notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func add(
    _ request: UNNotificationRequest,
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func add(_ request: UNNotificationRequest) async throws
```

## Parameters 

`request`  

The request object containing the notification payload and trigger information. This parameter must not be `nil`.

`completionHandler`  

The block to execute with the results. This block may be executed on a background thread. The block has no return value and takes the following parameter:

error  
An error object indicating whether a problem occurred. If the notification was scheduled successfully, this parameter is `nil`; otherwise, it is set to an error object indicating the reason for the failure.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func add(_ request: UNNotificationRequest) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method schedules local notifications only; you cannot use it to schedule the delivery of remote notifications. Upon calling this method, the system begins tracking the trigger conditions associated with your request. When the trigger condition is met, the system delivers your notification. If the request does not contain a UNNotificationTrigger object, the notification is delivered right away.

You may call this method from any thread of your app.

```
let center = UNUserNotificationCenter.current()
let content = UNMutableNotificationContent()
content.title = "My notification title"
content.body = "My notification body"
let notification = UNNotificationRequest(identifier: "com.example.mynotification", content: content, trigger: nil)
do {
    try await center.add(notification)
} catch {
    // Handle any errors.
}
```

## See Also

### Scheduling notifications

func getPendingNotificationRequests(completionHandler: ([UNNotificationRequest]) -> Void)

Fetches all of your app’s local notifications that are pending delivery.

func removePendingNotificationRequests(withIdentifiers: [String])

Removes your app’s local notifications that are pending and match the specified identifiers.

func removeAllPendingNotificationRequests()

Removes all of your app’s pending local notifications.

