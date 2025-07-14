

- AppKit
- NSCollectionViewTransitionLayout
-  NSCollectionViewTransitionLayout.AnimatedKey 

Type Alias

# NSCollectionViewTransitionLayout.AnimatedKey

macOS

``` source
typealias AnimatedKey = String
```

## See Also

### Updating the Transition Information

var transitionProgress: CGFloat

The completion percentage of the transition.

func updateValue(CGFloat, forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey)

Sets the value of a key whose value you use during the animation.

func value(forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey) -> CGFloat

Returns the most recently set value for the specified key.

