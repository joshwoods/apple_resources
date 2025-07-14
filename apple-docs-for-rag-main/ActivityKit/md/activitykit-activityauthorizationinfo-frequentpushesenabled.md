

- ActivityKit
- ActivityAuthorizationInfo
-  frequentPushesEnabled 

Instance Property

# frequentPushesEnabled

A Boolean value that indicates whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

iOS 16.2+iPadOS 16.2+

``` source
final var frequentPushesEnabled: Bool { get }
```

## Mentioned in 

Starting and updating Live Activities with ActivityKit push notifications

## See Also

### Observing availability of frequent ActivityKit push notifications

let frequentPushEnablementUpdates: ActivityAuthorizationInfo.FrequentPushEnablementUpdates

An asynchronous sequence you use to observe whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

struct FrequentPushEnablementUpdates

A structure that can observe whether you can update Live Activities with frequent ActivityKit push notifications.

