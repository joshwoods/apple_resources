

- Accelerate
-  BNNSOptimizerClippingNone 

Global Variable

# BNNSOptimizerClippingNone

A constant that specifes no clipping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var BNNSOptimizerClippingNone: BNNSOptimizerClippingFunction { get }
```

## See Also

### Clipping Functions

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSOptimizerClippingByValue: BNNSOptimizerClippingFunction

A constant that specifes clipping to minimum and maximum values.

var BNNSOptimizerClippingByNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum Euclidean norm.

var BNNSOptimizerClippingByGlobalNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum global Euclidean norm.

