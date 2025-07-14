

- UIKit
- UISlider
-  maximumValue 

Instance Property

# maximumValue

The maximum value of the slider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var maximumValue: Float { get set }
```

## Discussion

Use this property to set the value that the trailing end of the slider represents. If you change the value of this property, and the current value of the slider is above the new maximum, the slider adjusts the value property to match the new maximum. If you set the maximum value to a value smaller than the minimum, the slider updates the minimum value to equal the maximum.

The default value of this property is 1.0.

## See Also

### Accessing the slider’s value limits

var minimumValue: Float

The minimum value of the slider.

