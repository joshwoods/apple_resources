

- AppKit
- NSCollectionViewTransitionLayout
-  value(forAnimatedKey:) 

Instance Method

# value(forAnimatedKey:)

Returns the most recently set value for the specified key.

macOS 10.11+

``` source
@MainActor
func value(forAnimatedKey key: NSCollectionViewTransitionLayout.AnimatedKey) -> CGFloat
```

## Parameters 

`key`  

A key whose value you set previously using the updateValue(_:forAnimatedKey:) method.

## Return Value

The last value set for the key.

## Discussion

Use this method to retrieve floating-point values that relate to laying out the contents of your collection view. The key you specify is a string that you define and that has some meaning to your layout’s implementation. At points during an interactive transition, you can assign new values to that key using the updateValue(_:forAnimatedKey:) method.

## See Also

### Updating the Transition Information

var transitionProgress: CGFloat

The completion percentage of the transition.

func updateValue(CGFloat, forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey)

Sets the value of a key whose value you use during the animation.

typealias AnimatedKey

