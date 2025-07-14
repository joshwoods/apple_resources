

- UIKit
- UISlider
-  value 

Instance Property

# value

The slider’s current value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var value: Float { get set }
```

## Discussion

Use this property to get and set the slider’s current value. To render an animated transition from the current value to the new value, use the setValue(_:animated:) method instead.

If you try to set a value that’s below the minimum or above the maximum, the minimum or maximum value is set instead. The default value of this property is `0.0`.

## See Also

### Accessing the slider’s value

func setValue(Float, animated: Bool)

Sets the slider’s current value, allowing you to animate the change visually.

