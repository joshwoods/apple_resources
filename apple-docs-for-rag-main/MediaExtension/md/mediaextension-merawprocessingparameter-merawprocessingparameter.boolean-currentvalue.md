

- MediaExtension
- MERAWProcessingParameter
- MERAWProcessingParameter.Boolean
-  currentValue 

Instance Property

# currentValue

Get or set the current value for this parameter.

macOS 15.0+

``` source
var currentValue: Bool { get set }
```

## Discussion

This property can be observed if appropriate in order to monitor changes to the set of `MERAWProcessingParameters` vended by the extension.

## See Also

### Properties

var initialValue: Bool

The initial value for this parameter as defined in the sequence metadata.

