

- Core Haptics
- CHHapticEventParameter
-  value 

Instance Property

# value

The value of the parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var value: Float { get set }
```

## Discussion

The range of possible values varies between different parameters. For example, haptic intensity and haptic sharpness vary between `0` and `1`, with `0` indicating minimal intensity or sharpness, and `1` indicating the maximum intensity or sharpness value allowed. See the individual parameter pages for the ranges and default values of each parameter.

## See Also

### Specifying an Event Parameter’s Value

var parameterID: CHHapticEvent.ParameterID

The haptic parameter ID indicating what type of parameter the current event represents.

