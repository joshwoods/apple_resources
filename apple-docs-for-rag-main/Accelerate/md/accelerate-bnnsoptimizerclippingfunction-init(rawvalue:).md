

- Accelerate
- BNNSOptimizerClippingFunction
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(rawValue: UInt32)
```

## See Also

### Clipping Functions

init(UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSOptimizerClippingNone: BNNSOptimizerClippingFunction

A constant that specifes no clipping.

var BNNSOptimizerClippingByValue: BNNSOptimizerClippingFunction

A constant that specifes clipping to minimum and maximum values.

var BNNSOptimizerClippingByNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum Euclidean norm.

var BNNSOptimizerClippingByGlobalNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum global Euclidean norm.

