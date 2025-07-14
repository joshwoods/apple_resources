

- AppKit
- NSCollectionViewTransitionLayout
-  updateValue(\_:forAnimatedKey:) 

Instance Method

# updateValue(\_:forAnimatedKey:)

Sets the value of a key whose value you use during the animation.

macOS 10.11+

``` source
@MainActor
func updateValue(
    _ value: CGFloat,
    forAnimatedKey key: NSCollectionViewTransitionLayout.AnimatedKey
)
```

## Parameters 

`value`  

The value of the key.

`key`  

The key that you define for your custom transition layout.

## Discussion

Use this method to update the value of a specific key that you use in your custom transition layout.

## See Also

### Updating the Transition Information

var transitionProgress: CGFloat

The completion percentage of the transition.

func value(forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey) -> CGFloat

Returns the most recently set value for the specified key.

typealias AnimatedKey

