

- Audio Toolbox
- AUParameter
-  dependentParameters 

Instance Property

# dependentParameters

Any other parameter’s whose values may change as a side effect of this parameter’s value changing.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var dependentParameters: [NSNumber]? { get }
```

## Discussion

The array contains NSNumber objects representing AUParameterAddress values.

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

var valueStrings: [String]?

The parameter’s localized value strings.

