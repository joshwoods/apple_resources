

- ActivityKit
- Activity
-  pushTokenUpdates 

Instance Property

# pushTokenUpdates

An asynchronous sequence you use to observe changes to the push token of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
var pushTokenUpdates: Activity.PushTokenUpdates { get }
```

## Mentioned in 

Displaying live data with Live Activities

Starting and updating Live Activities with ActivityKit push notifications

## See Also

### Using ActivityKit push notifications

var pushToken: Data?

The token you use to send ActivityKit push notifications to a Live Activity.

struct PushTokenUpdates

A structure that offers functionality to observe changes to the push token of a Live Activity.

static var pushToStartToken: Data?

The token you use to start a Live Activity with an ActivityKit push notification.

static var pushToStartTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the token for starting a Live Activity with an ActivityKit push notification.

