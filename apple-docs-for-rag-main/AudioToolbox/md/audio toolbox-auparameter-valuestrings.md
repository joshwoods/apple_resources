

- Audio Toolbox
- AUParameter
-  valueStrings 

Instance Property

# valueStrings

The parameter’s localized value strings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var valueStrings: [String]? { get }
```

## Discussion

This property allows you to specify an array of strings to be used for the values of an indexed parameter—for example, a *band* parameter could publish these values: “High”, “Medium”, “Low”.

## See Also

### Querying Parameter Properties

var minValue: AUValue

The parameter’s minimum value.

var maxValue: AUValue

The parameter’s maximum value.

var unit: AudioUnitParameterUnit

The parameter’s unit of measurement.

var unitName: String?

The parameter’s localized unit name.

var flags: AudioUnitParameterOptions

The parameter’s characteristic details.

var address: AUParameterAddress

The parameter’s address.

var dependentParameters: [NSNumber]?

Any other parameter’s whose values may change as a side effect of this parameter’s value changing.

