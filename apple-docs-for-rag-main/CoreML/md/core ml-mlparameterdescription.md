

- Core ML
-  MLParameterDescription 

Class

# MLParameterDescription

A description of a model parameter that includes a default value and a constraint, if applicable.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLParameterDescription
```

## Topics

### Describing the Model Parameter

var defaultValue: Any

The default value for the parameter.

var key: MLParameterKey

The key for this parameter description value.

### Constraining Numeric Values

var numericConstraint: MLNumericConstraint?

The constraints of this paramter description value, if and only if the value is numerical.

class MLNumericConstraint

The value limitations of a number.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing Update Descriptions

var isUpdatable: Bool

A Boolean value that indicates whether you can update the model with additional training.

var trainingInputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of the training input feature descriptions, which the model keys by the input’s name.

var parameterDescriptionsByKey: [MLParameterKey : MLParameterDescription]

A dictionary of the descriptions for the model’s parameters.

