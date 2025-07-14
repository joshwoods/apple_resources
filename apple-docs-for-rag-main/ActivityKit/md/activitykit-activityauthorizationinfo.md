

- ActivityKit
-  ActivityAuthorizationInfo 

Class

# ActivityAuthorizationInfo

An object with information about whether a person allowed your app to start Live Activities and permitted content updates with frequent ActivityKit push notifications.

iOS 16.1+iPadOS 16.1+

``` source
final class ActivityAuthorizationInfo
```

## Overview

By default, your app can start, update, and end a Live Activity if you use ActivityKit to offer Live Activities. However, a person can deactivate Live Activities for an app in Settings. To check if your app can start, update, or end a Live Activity, use the synchronous areActivitiesEnabled property or the asynchronous activityEnablementUpdates sequence.

Similarly, `ActivityAuthorizationInfo` provides functionality to check whether a person has permitted your app to update Live Activities with frequent ActivityKit push notifications. To check whether you can send frequent ActivityKit push notifications to update Live Activity content, use the synchronous frequentPushesEnabled property or the asynchronous frequentPushEnablementUpdates sequence.

Note

To update a Live Activity with frequent ActivityKit push notifications, add the `NSSupportsFrequentLiveActivityUpdates` key with a Boolean value of `YES` to your app’s `Info.plist` file. For additional information, see Starting and updating Live Activities with ActivityKit push notifications.

## Topics

### Observing Live Activity permission changes

var areActivitiesEnabled: Bool

A Boolean value that indicates whether your app can start a Live Activity.

let activityEnablementUpdates: ActivityAuthorizationInfo.ActivityEnablementUpdates

An asynchronous sequence you use to observe whether your app can start a Live Activity.

struct ActivityEnablementUpdates

A structure that offers functionality to observe whether your app can start a Live Activity.

init()

Creates an object you use to observe user authorizations for starting Live Activities and updating them with ActivityKit push notifications.

### Observing availability of frequent ActivityKit push notifications

var frequentPushesEnabled: Bool

A Boolean value that indicates whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

let frequentPushEnablementUpdates: ActivityAuthorizationInfo.FrequentPushEnablementUpdates

An asynchronous sequence you use to observe whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

struct FrequentPushEnablementUpdates

A structure that can observe whether you can update Live Activities with frequent ActivityKit push notifications.

