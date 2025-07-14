

- ActivityKit
- ActivityAuthorizationInfo
-  init() 

Initializer

# init()

Creates an object you use to observe user authorizations for starting Live Activities and updating them with ActivityKit push notifications.

iOS 16.1+iPadOS 16.1+

``` source
init()
```

## See Also

### Observing Live Activity permission changes

var areActivitiesEnabled: Bool

A Boolean value that indicates whether your app can start a Live Activity.

let activityEnablementUpdates: ActivityAuthorizationInfo.ActivityEnablementUpdates

An asynchronous sequence you use to observe whether your app can start a Live Activity.

struct ActivityEnablementUpdates

A structure that offers functionality to observe whether your app can start a Live Activity.

