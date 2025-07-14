

- Accelerate
- BNNSActivation
-  integerLinearSaturate(scale:offset:shift:) Deprecated

Type Method

# integerLinearSaturate(scale:offset:shift:)

Returns an activation function that computes an arithmetic shift, preserving sign.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+visionOSwatchOS 4.0+tvOS 11.0+

``` source
static func integerLinearSaturate(
    scale: Int32 = 1,
    offset: Int32 = 0,
    shift: Int32 = 0
) -> BNNSActivation
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`scale`  

The scale for the activation function.

`offset`  

The offset for the activation function.

`shift`  

The arithmetic shift for the activation function.

## See Also

### Related Documentation

BNNSActivationFunctionIntegerLinearSaturate

An activation function that returns an arithmetic shift, preserving sign.

### Type Methods

static func integerLinearSaturatePerChannel(scale: UnsafePointer&lt;Int32>, offset: UnsafePointer&lt;Int32>, shift: UnsafePointer&lt;Int32>) -> BNNSActivation

Returns an activation function that computes an arithmetic shift, preserving sign for each channel.

Deprecated

