

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
-  MLStyleTransfer.ModelParameters.ValidationData 

Enumeration

# MLStyleTransfer.ModelParameters.ValidationData

The source of a validation dataset for a style transfer model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ValidationData
```

## Topics

### Designating validation data

case content(URL)

The location of a validation image you use to validate the model.

case none

An empty validation dataset you use to skip model validation.

### Comparing validation data

static func == (MLStyleTransfer.ModelParameters.ValidationData, MLStyleTransfer.ModelParameters.ValidationData) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Describing parameters

enum ModelAlgorithmType

The style transfer training algorithm options.

