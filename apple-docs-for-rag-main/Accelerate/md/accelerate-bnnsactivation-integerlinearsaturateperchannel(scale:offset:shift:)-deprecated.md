

- Accelerate
- BNNSActivation
-  integerLinearSaturatePerChannel(scale:offset:shift:) Deprecated

Type Method

# integerLinearSaturatePerChannel(scale:offset:shift:)

Returns an activation function that computes an arithmetic shift, preserving sign for each channel.

iOS 11.0+iPadOS 11.0+macOS 10.13+tvOS 11.0+visionOSwatchOS 4.0+Mac Catalyst

``` source
static func integerLinearSaturatePerChannel(
    scale: UnsafePointer,
    offset: UnsafePointer,
    shift: UnsafePointer
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

BNNSActivationFunctionIntegerLinearSaturatePerChannel

An activation function that returns an arithmetic shift, preserving sign for each channel.

### Type Methods

static func integerLinearSaturate(scale: Int32, offset: Int32, shift: Int32) -> BNNSActivation

Returns an activation function that computes an arithmetic shift, preserving sign.

Deprecated

