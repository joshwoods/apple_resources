

- ActivityKit
- Activity
-  pushToken 

Instance Property

# pushToken

The token you use to send ActivityKit push notifications to a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
var pushToken: Data? { get }
```

## Mentioned in 

Starting and updating Live Activities with ActivityKit push notifications

## Discussion

The push token for a Live Activity may change over time. Use the pushTokenUpdates asynchronous sequence to receive the updated push token. When you receive an updated push token, make sure to send it to your server and invalidate the outdated token.

## See Also

### Using ActivityKit push notifications

var pushTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the push token of a Live Activity.

struct PushTokenUpdates

A structure that offers functionality to observe changes to the push token of a Live Activity.

static var pushToStartToken: Data?

The token you use to start a Live Activity with an ActivityKit push notification.

static var pushToStartTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the token for starting a Live Activity with an ActivityKit push notification.

