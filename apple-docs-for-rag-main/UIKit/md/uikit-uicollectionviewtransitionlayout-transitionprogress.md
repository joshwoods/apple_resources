

- UIKit
- UICollectionViewTransitionLayout
-  transitionProgress 

Instance Property

# transitionProgress

The completion percentage of the transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var transitionProgress: CGFloat { get set }
```

## Discussion

During the transition, you should set the value of this property periodically and call invalidateLayout() to force the collection view to update item positions. If you are driving the transition with a gesture recognizer, you would likely set this property from the handler method of your gesture recognizer.

## See Also

### Updating the transition information

func updateValue(CGFloat, forAnimatedKey: String)

Sets the value for an animatable key.

func value(forAnimatedKey: String) -> CGFloat

Returns the most recently set value for the specified key.

