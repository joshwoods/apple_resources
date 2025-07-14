

- AppKit
- NSCollectionViewTransitionLayout
-  transitionProgress 

Instance Property

# transitionProgress

The completion percentage of the transition.

macOS 10.11+

``` source
@MainActor
var transitionProgress: CGFloat { get set }
```

## Discussion

During the transition, set the value of this property periodically and call the invalidateLayout() method to force the collection view to update item positions. For example, when driving a transition using a gesture recognizer, you can set this property from the handler method of your gesture recognizer.

## See Also

### Updating the Transition Information

func updateValue(CGFloat, forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey)

Sets the value of a key whose value you use during the animation.

func value(forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey) -> CGFloat

Returns the most recently set value for the specified key.

typealias AnimatedKey

