

- UIKit
- UISceneCollectionJoinBehavior
-  UISceneCollectionJoinBehavior.disallowed 

Case

# UISceneCollectionJoinBehavior.disallowed

A behavior that creates a new collection for the new scene, ignoring system preferences.

Mac Catalyst 14.0+

``` source
case disallowed
```

## See Also

### Constants

case automatic

A behavior that uses the system preferences for joining collections.

case preferred

A behavior that adds the new scene to the requesting scene’s collection and activate it, or attempts to join a compatible collection.

case preferredWithoutActivating

A behavior that adds the new scene to the requesting scene’s collection without activating it, or attempts to join a compatible collection.

