

- UIKit
- UICollectionViewTransitionLayout
-  updateValue(\_:forAnimatedKey:) 

Instance Method

# updateValue(\_:forAnimatedKey:)

Sets the value for an animatable key.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func updateValue(
    _ value: CGFloat,
    forAnimatedKey key: String
)
```

## Parameters 

`value`  

The value you want to store for the specified key.

`key`  

A key that you define for your custom transition layout.

## Discussion

Use this method to store a floating-point value with a specific key that you define for your transition layout object. The name of the key should be one that has meaning to your layout object. For example, if you track the position of the user’s finger over time, you might define the keys “PositionX” and “PositionY” to track those changes. Each time you update the value of a key, the layout object records the change along with a timestamp value. When the layout is finalized or canceled, those values can then be used to determine the speed with which to perform the remaining animations.

For any keys you set using this method, you should get that value as part of the normal process of generating layout attribute information. Getting the value using the value(forAnimatedKey:) method (as opposed to getting the value from a class variable) means that when the collection view performs its final animations, your layout methods provide the correct values.

## See Also

### Updating the transition information

var transitionProgress: CGFloat

The completion percentage of the transition.

func value(forAnimatedKey: String) -> CGFloat

Returns the most recently set value for the specified key.

