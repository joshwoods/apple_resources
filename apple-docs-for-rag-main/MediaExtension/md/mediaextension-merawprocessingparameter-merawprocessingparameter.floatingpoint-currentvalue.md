

- MediaExtension
- MERAWProcessingParameter
- MERAWProcessingParameter.FloatingPoint
-  currentValue 

Instance Property

# currentValue

Get or set the current value for this parameter.

macOS 15.0+

``` source
var currentValue: Float { get set }
```

## Discussion

This property can be observed if appropriate in order to monitor changes to the set of `MERAWProcessingParameters` vended by the extension.

## See Also

### Properties

var initialValue: Float

The initial value for this parameter as defined in the sequence metadata.

var maximumValue: Float

The maximum value for this parameter.

var minimumValue: Float

The minimum value for this parameter.

