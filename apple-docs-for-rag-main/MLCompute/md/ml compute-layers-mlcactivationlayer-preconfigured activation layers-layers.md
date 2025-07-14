

- ML Compute
- Layers
- MLCActivationLayer
-  Preconfigured Activation Layers 

API Collection

# Preconfigured Activation Layers

Obtain a preconfigured activation layer with common behavior.

## Overview

Use a factory to receive a preconfigured activation layer for various activation types.

## Topics

### Factory Methods

class func celu(a: Float) -> Self

Creates an instance of a CELU activation layer using the alpha value you specify for the CELU formation.

Deprecated

class func clamp(min: Float, max: Float) -> Self

Creates an instance of a clamp activation layer using the minimum and maximum values you specify for the clamp formation.

Deprecated

class func elu(a: Float) -> Self

Creates an instance of an ELU activation layer using the alpha value you specify for the ELU formation.

Deprecated

class func hardShrink(a: Float) -> Self

Creates an instance of a hard shrink activation layer using the lambda value you specify for the hard shrink formation.

Deprecated

class func leakyReLU(negativeSlope: Float) -> Self

Creates an instance of a leaky ReLU activation layer using the angle of the negative slope you specify.

Deprecated

class func linear(scale: Float, bias: Float) -> Self

Creates an instance of a linear activation layer using the scale factor and bias value you specify.

Deprecated

class func relun(a: Float, b: Float) -> Self

Creates an instance of a ReLUN activation layer using the alpha and beta values you specify.

Deprecated

class func softPlus(beta: Float) -> Self

Creates an instance of a soft plus activation layer using the beta value you specify for the soft plus formation.

Deprecated

class func softShrink(a: Float) -> Self

Creates an instance of a soft shrink activation layer using the lambda value you specify for the soft shrink formation.

Deprecated

class func threshold(Float, replacement: Float) -> Self

Creates an instance of a threshold activation layer using the threshold and replacement values you specify.

Deprecated

### Factory Properties

class var absolute: MLCActivationLayer

Creates an instance of an absolute activation layer.

Deprecated

class var celu: MLCActivationLayer

Creates an instance of a CELU activation layer.

Deprecated

class var elu: MLCActivationLayer

Creates an instance of a parametric ELU activation layer.

Deprecated

class var gelu: MLCActivationLayer

Creates an instance of a GELU activation layer.

Deprecated

class var hardShrink: MLCActivationLayer

Creates an instance of a hard shrink activation layer.

Deprecated

class var hardSigmoid: MLCActivationLayer

Creates an instance of a hard sigmoid activation layer.

Deprecated

class var hardSwish: MLCActivationLayer

Creates an instance of a hard swish activation layer.

Deprecated

class var leakyReLU: MLCActivationLayer

Creates an instance of a leaky ReLU activation layer.

Deprecated

class var logSigmoid: MLCActivationLayer

Creates an instance of a log sigmoid activation layer.

Deprecated

class var relu: MLCActivationLayer

Creates an instance of a ReLU activation layer.

Deprecated

class var relu6: MLCActivationLayer

Creates an instance of a ReLU6 activation layer.

Deprecated

class var selu: MLCActivationLayer

Creates an instance of a SELU activation layer.

Deprecated

class var sigmoid: MLCActivationLayer

Creates an instance of a sigmoid activation layer.

Deprecated

class var softPlus: MLCActivationLayer

Creates an instance of a parametric soft plus activation layer.

Deprecated

class var softShrink: MLCActivationLayer

Creates an instance of a soft shrink activation layer.

Deprecated

class var softSign: MLCActivationLayer

Creates an instance of a parametric soft sign activation layer.

Deprecated

class var tanh: MLCActivationLayer

Creates an instance of a hyperbolic tangent activation layer.

Deprecated

class var tanhShrink: MLCActivationLayer

Creates an instance of a tanh shrink activation layer.

Deprecated

## See Also

### Creating Activation Layers

convenience init(descriptor: MLCActivationDescriptor)

Creates an activation layer with the descriptor you specify.

Deprecated

class MLCActivationDescriptor

A configuration object you use to create an activation layer.

Deprecated

