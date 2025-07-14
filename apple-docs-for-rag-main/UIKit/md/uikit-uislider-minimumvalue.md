

- UIKit
- UISlider
-  minimumValue 

Instance Property

# minimumValue

The minimum value of the slider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var minimumValue: Float { get set }
```

## Discussion

Use this property to set the value that the leading end of the slider represents. If you change the value of this property, and the current value of the slider is below the new minimum, the slider adjusts the value property to match the new minimum. If you set the minimum value to a value larger than the maximum, the slider updates the maximum value to equal the minimum.

The default value of this property is 0.0.

## See Also

### Accessing the slider’s value limits

var maximumValue: Float

The maximum value of the slider.

