

- UIKit
- UISceneCollectionJoinBehavior
-  UISceneCollectionJoinBehavior.preferred 

Case

# UISceneCollectionJoinBehavior.preferred

A behavior that adds the new scene to the requesting scene’s collection and activate it, or attempts to join a compatible collection.

Mac Catalyst 14.0+

``` source
case preferred
```

## Discussion

If requestingScene is set, this behavior adds the new scene to its collection and activates it. Otherwise, the scene attempts to join a compatible collection.

## See Also

### Constants

case automatic

A behavior that uses the system preferences for joining collections.

case preferredWithoutActivating

A behavior that adds the new scene to the requesting scene’s collection without activating it, or attempts to join a compatible collection.

case disallowed

A behavior that creates a new collection for the new scene, ignoring system preferences.

