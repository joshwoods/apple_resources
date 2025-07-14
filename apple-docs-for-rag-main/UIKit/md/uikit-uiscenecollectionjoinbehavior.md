

- UIKit
-  UISceneCollectionJoinBehavior 

Enumeration

# UISceneCollectionJoinBehavior

A set of behaviors that specify how a new scene joins a scene collection.

Mac Catalyst 14.0+

``` source
enum UISceneCollectionJoinBehavior
```

## Topics

### Constants

case automatic

A behavior that uses the system preferences for joining collections.

case preferred

A behavior that adds the new scene to the requesting scene’s collection and activate it, or attempts to join a compatible collection.

case preferredWithoutActivating

A behavior that adds the new scene to the requesting scene’s collection without activating it, or attempts to join a compatible collection.

case disallowed

A behavior that creates a new collection for the new scene, ignoring system preferences.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying collection join behavior

var collectionJoinBehavior: UISceneCollectionJoinBehavior

The behavior that specifies how a new scene joins a scene collection.

