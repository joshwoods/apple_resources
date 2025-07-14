

- ActivityKit
- Activity
-  pushToStartToken 

Type Property

# pushToStartToken

The token you use to start a Live Activity with an ActivityKit push notification.

iOS 17.2+iPadOS 17.2+

``` source
static var pushToStartToken: Data? { get }
```

## Discussion

The push token for a Live Activity may change over time. Use the pushToStartTokenUpdates asynchronous sequence to receive an updated push-to-start token. When you receive an updated push token, make sure to send it to your server and invalidate the outdated token.

## See Also

### Using ActivityKit push notifications

var pushToken: Data?

The token you use to send ActivityKit push notifications to a Live Activity.

var pushTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the push token of a Live Activity.

struct PushTokenUpdates

A structure that offers functionality to observe changes to the push token of a Live Activity.

static var pushToStartTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the token for starting a Live Activity with an ActivityKit push notification.

