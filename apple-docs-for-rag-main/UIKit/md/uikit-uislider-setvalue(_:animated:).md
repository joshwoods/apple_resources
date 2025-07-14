

- UIKit
- UISlider
-  setValue(\_:animated:) 

Instance Method

# setValue(\_:animated:)

Sets the slider’s current value, allowing you to animate the change visually.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setValue(
    _ value: Float,
    animated: Bool
)
```

## Parameters 

`value`  

The new value to assign to the value property

`animated`  

Specify true to animate the change in value; otherwise, specify false to update the slider’s appearance immediately. Animations are performed asynchronously and do not block the calling thread.

## Discussion

If you specify a value that is beyond the minimum or maximum values, the slider limits the value to the minimum or maximum. For example, if the minimum value is 0.0 and you specify -1.0, the slider sets the value property to 0.0.

## See Also

### Accessing the slider’s value

var value: Float

The slider’s current value.

