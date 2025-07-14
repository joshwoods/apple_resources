

- User Notifications
- UNUserNotificationCenter
-  setBadgeCount(\_:withCompletionHandler:) 

Instance Method

# setBadgeCount(\_:withCompletionHandler:)

Updates the badge count for your app’s icon.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setBadgeCount(
    _ newBadgeCount: Int,
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setBadgeCount(_ newBadgeCount: Int) async throws
```

## Parameters 

`newBadgeCount`  

The new value to display.

`completionHandler`  

The handler to execute after the update finishes. If the update fails, the system provides an error that contains additional information about the failure.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setBadgeCount(_ newBadgeCount: Int) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Here’s an example that sets the badge count to a specific number.

```
let center = UNUserNotificationCenter.current()
do {
     // Set the badge count to 3.
     try await center.setBadgeCount(3)
} catch {
     // Handle any errors.
}
```

## See Also

### Managing the notification center

class func current() -> UNUserNotificationCenter

Returns your app’s notification center.

func getNotificationSettings(completionHandler: (UNNotificationSettings) -> Void)

Retrieves the authorization and feature-related settings for your app.

