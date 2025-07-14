

- Accelerate
- BNNS
-  BNNS.ConvolutionPadding Deprecated

Enumeration

# BNNS.ConvolutionPadding

Constants that describe convolution padding modes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
enum ConvolutionPadding
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Convolution Padding Modes

case asymmetric(left: Int, right: Int, up: Int, down: Int)

A padding mode that supports individual padding values for each side.

case symmetric(x: Int, y: Int)

A padding mode that provides symmetric padding.

### Special Values

static var zero: BNNS.ConvolutionPadding

A padding mode with zero padding on all sides.

