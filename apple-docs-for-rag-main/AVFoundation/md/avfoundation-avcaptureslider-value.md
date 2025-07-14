

- AVFoundation
- AVCaptureSlider
-  value 

Instance Property

# value

The current value of the slider.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var value: Float { get set }
```

## Discussion

The default value is the slider’s minimum value. You may set a value only if it’s within the slider’s minimum and maximum values, otherwise the system throws an exception.

Important

Only modify a slider’s value from the same dispatch queue that you specified in the control’s setActionQueue:action: method.

## See Also

### Accessing the control value

var prominentValues: [Float]

Values in this array may receive unique visual representations or behaviors.

var localizedValueFormat: String?

A localized string that defines the presentation of the slider’s value.

