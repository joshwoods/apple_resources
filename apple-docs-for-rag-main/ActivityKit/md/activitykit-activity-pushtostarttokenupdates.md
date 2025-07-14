

- ActivityKit
- Activity
-  pushToStartTokenUpdates 

Type Property

# pushToStartTokenUpdates

An asynchronous sequence you use to observe changes to the token for starting a Live Activity with an ActivityKit push notification.

iOS 17.2+iPadOS 17.2+

``` source
static var pushToStartTokenUpdates: Activity.PushTokenUpdates { get }
```

## Mentioned in 

Starting and updating Live Activities with ActivityKit push notifications

## Discussion

Starting with iOS 17.2, you can adopt push notifications to not only update ongoing Live Activities, but also to start a new Live Activity. For additional information, see Starting and updating Live Activities with ActivityKit push notifications.

## See Also

### Using ActivityKit push notifications

var pushToken: Data?

The token you use to send ActivityKit push notifications to a Live Activity.

var pushTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the push token of a Live Activity.

struct PushTokenUpdates

A structure that offers functionality to observe changes to the push token of a Live Activity.

static var pushToStartToken: Data?

The token you use to start a Live Activity with an ActivityKit push notification.

