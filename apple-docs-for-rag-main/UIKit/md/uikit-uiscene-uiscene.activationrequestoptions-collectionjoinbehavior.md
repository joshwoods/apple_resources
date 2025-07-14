

- UIKit
- UIScene
- UIScene.ActivationRequestOptions
-  collectionJoinBehavior 

Instance Property

# collectionJoinBehavior

The behavior that specifies how a new scene joins a scene collection.

Mac Catalyst 14.0+

``` source
@MainActor
var collectionJoinBehavior: UISceneCollectionJoinBehavior { get set }
```

## Discussion

A scene collection is a group of scenes that display together. In apps built with Mac Catalyst, you use this behavior to add windows to an NSWindowTabGroup.

## See Also

### Specifying collection join behavior

enum UISceneCollectionJoinBehavior

A set of behaviors that specify how a new scene joins a scene collection.

