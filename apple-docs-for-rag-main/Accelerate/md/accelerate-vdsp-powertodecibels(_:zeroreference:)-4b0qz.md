

- Accelerate
- vDSP
-  powerToDecibels(\_:zeroReference:) 

Type Method

# powerToDecibels(\_:zeroReference:)

Returns double-precision power values converted to decibel values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func powerToDecibels(
    _ power: U,
    zeroReference: Double
) -> [Double] where U : AccelerateBuffer, U.Element == Double
```

## Parameters 

`power`  

The input vector that defines the power values.

`zeroReference`  

The zero reference that the function uses for the conversion.

## Discussion

The function uses the following calculation to perform the conversion:

```
alpha = 10;

for (n = 0; n 

## See Also

### Converting double-precision power or amplitude values to decibel values

static func amplitudeToDecibels&lt;U>(U, zeroReference: Double) -> [Double]

Returns double-precision amplitude values converted to decibel values.

static func convert&lt;U, V>(amplitude: U, toDecibels: inout V, zeroReference: Double)

Converts double-precision amplitude values to decibel values.

static func convert&lt;U, V>(power: U, toDecibels: inout V, zeroReference: Double)

Converts double-precision power values to decibel values.

