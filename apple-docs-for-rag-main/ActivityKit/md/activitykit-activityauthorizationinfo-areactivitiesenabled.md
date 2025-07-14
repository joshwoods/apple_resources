

- ActivityKit
- ActivityAuthorizationInfo
-  areActivitiesEnabled 

Instance Property

# areActivitiesEnabled

A Boolean value that indicates whether your app can start a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
final var areActivitiesEnabled: Bool { get }
```

## Mentioned in 

Displaying live data with Live Activities

## See Also

### Observing Live Activity permission changes

let activityEnablementUpdates: ActivityAuthorizationInfo.ActivityEnablementUpdates

An asynchronous sequence you use to observe whether your app can start a Live Activity.

struct ActivityEnablementUpdates

A structure that offers functionality to observe whether your app can start a Live Activity.

init()

Creates an object you use to observe user authorizations for starting Live Activities and updating them with ActivityKit push notifications.

