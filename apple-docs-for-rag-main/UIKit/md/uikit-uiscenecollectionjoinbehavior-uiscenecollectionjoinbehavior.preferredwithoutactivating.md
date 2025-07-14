

- UIKit
- UISceneCollectionJoinBehavior
-  UISceneCollectionJoinBehavior.preferredWithoutActivating 

Case

# UISceneCollectionJoinBehavior.preferredWithoutActivating

A behavior that adds the new scene to the requesting scene’s collection without activating it, or attempts to join a compatible collection.

Mac Catalyst 14.0+

``` source
case preferredWithoutActivating
```

## Discussion

If requestingScene is set, this behavior adds the new scene without deactivating the requestingScene. Otherwise, this behavior behaves the same as UISceneCollectionJoinBehavior.preferred. For example, in apps built with Mac Catalyst, you can use this behavior to open a link in a new tab in the background.

## See Also

### Constants

case automatic

A behavior that uses the system preferences for joining collections.

case preferred

A behavior that adds the new scene to the requesting scene’s collection and activate it, or attempts to join a compatible collection.

case disallowed

A behavior that creates a new collection for the new scene, ignoring system preferences.

