

- ML Compute
-  MLCActivationType Deprecated

Enumeration

# MLCActivationType

An activation type that you specify for an activation descriptor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCActivationType
```

## Topics

### Enumeration Cases

case absolute

An activation type that implements the absolute activation function.

case celu

An activation type that implements the CELU activation function.

case clamp

An activation type that implements the clamp activation function.

case elu

An activation type that implements the exponential linear unit activation function.

case gelu

An activation type that implements the gaussian error linear unit activation function.

case hardShrink

An activation type that implements the hard shrink activation function.

case hardSigmoid

An activation type that implements the hard sigmoid activation function.

case hardSwish

An activation type that implements the hard swish activation function.

case linear

An activation type that implements the linear activation function.

case logSigmoid

An activation type that implements the log sigmoid activation function.

case none

An activation type that implements the identity function.

case relu

An activation type that implements the rectified linear unit activation function.

case relun

An activation type that implements the ReLUN activation function.

case selu

An activation type that implements the scaled exponential linear unit activation function.

case sigmoid

An activation type that implements the sigmoid activation function.

case softPlus

An activation type that implements the soft plus activation function.

case softShrink

An activation type that implements the soft shrink activation function.

case softSign

An activation type that implements the parametric soft sign activation function.

case tanh

An activation type that implements the hyperbolic tangent activation function.

case tanhShrink

An activation type that implements the hyperbolic tangent shrink activation function.

case threshold

An activation type that implements the threshold activation function.

var debugDescription: String

A textual description of the activation type, suitable for debugging.

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

### Creating Activation Descriptors

convenience init?(type: MLCActivationType)

Creates an activation descriptor with the activation type you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float)

Creates an activation descriptor with the activation type and parameter a that you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float)

Creates an activation descriptor with the activation type and parameters a and b that you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float, c: Float)

Creates an activation descriptor with the activation type and parameters a, b, and c that you specify.

Deprecated

