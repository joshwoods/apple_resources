

- ML Compute
- MLCActivationLayer
-  selu Deprecated

Type Property

# selu

Creates an instance of a SELU activation layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class var selu: MLCActivationLayer { get }
```

## Discussion

This factory creates an activation descriptor using init(type:), where `type =` MLCActivationType.selu, and passes that descriptor to init(descriptor:).

## See Also

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

