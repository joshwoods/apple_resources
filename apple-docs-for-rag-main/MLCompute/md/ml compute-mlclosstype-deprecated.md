

- ML Compute
-  MLCLossType Deprecated

Enumeration

# MLCLossType

A loss function.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCLossType
```

## Topics

### Enumeration Cases

case categoricalCrossEntropy

case cosineDistance

case hinge

case huber

case log

case meanAbsoluteError

case meanSquaredError

case sigmoidCrossEntropy

case softmaxCrossEntropy

var debugDescription: String

A textual description of the loss type, suitable for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Loss Layers with Descriptors

convenience init(descriptor: MLCLossDescriptor)

Creates a loss layer with the descriptor you specify.

Deprecated

convenience init(descriptor: MLCLossDescriptor, weights: MLCTensor)

Creates a loss layer with the descriptor and weights you specify.

Deprecated

class MLCLossDescriptor

A configuration object you use to create a loss layer.

Deprecated

