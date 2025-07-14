

- ML Compute
-  MLCActivationDescriptor Deprecated

Class

# MLCActivationDescriptor

A configuration object you use to create an activation layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCActivationDescriptor
```

## Overview

The framework provides the following activation descriptor initializers to create the associated descriptors:

init(type:)  
Absolute, GELU, Identity, LogSigmoid, Parametric Soft Sign, SELU, Sigmoid, TanhShrink

init(type:a:)  
CELU, HardShrink, Parametric ELU, ReLU, SoftShrink

init(type:a:b:)  
Hard Sigmoid, Hyperbolic tangent (TanH), Linear, Parametric Soft Plus, ReLUN, Threshold

## Topics

### Creating Activation Descriptors

convenience init?(type: MLCActivationType)

Creates an activation descriptor with the activation type you specify.

convenience init?(type: MLCActivationType, a: Float)

Creates an activation descriptor with the activation type and parameter a that you specify.

convenience init?(type: MLCActivationType, a: Float, b: Float)

Creates an activation descriptor with the activation type and parameters a and b that you specify.

convenience init?(type: MLCActivationType, a: Float, b: Float, c: Float)

Creates an activation descriptor with the activation type and parameters a, b, and c that you specify.

enum MLCActivationType

An activation type that you specify for an activation descriptor.

### Inspecting Activation Descriptors

var activationType: MLCActivationType

The type of activation function.

var a: Float

The parameter a to the activation function.

var b: Float

The parameter b to the activation function.

var c: Float

The parameter c to the activation function.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating Activation Layers

convenience init(descriptor: MLCActivationDescriptor)

Creates an activation layer with the descriptor you specify.

Deprecated

Preconfigured Activation Layers

Obtain a preconfigured activation layer with common behavior.

