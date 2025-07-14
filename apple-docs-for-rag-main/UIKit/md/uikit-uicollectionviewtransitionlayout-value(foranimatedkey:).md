

- UIKit
- UICollectionViewTransitionLayout
-  value(forAnimatedKey:) 

Instance Method

# value(forAnimatedKey:)

Returns the most recently set value for the specified key.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func value(forAnimatedKey key: String) -> CGFloat
```

## Parameters 

`key`  

A key whose value you set using the updateValue(_:forAnimatedKey:) method.

## Return Value

The last value set for the key.

## Discussion

Use this method to retrieve floating-point values that are useful when laying out the contents of your collection view. The key you specify is a string that you define and that has some meaning to your implementation. At points during an interactive transition, you can assign new values to that key using the updateValue(_:forAnimatedKey:) method.

## See Also

### Updating the transition information

var transitionProgress: CGFloat

The completion percentage of the transition.

func updateValue(CGFloat, forAnimatedKey: String)

Sets the value for an animatable key.

