

- Accelerate
- vDSP
-  convert(amplitude:toDecibels:zeroReference:) 

Type Method

# convert(amplitude:toDecibels:zeroReference:)

Converts double-precision amplitude values to decibel values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convert(
    amplitude: U,
    toDecibels decibels: inout V,
    zeroReference: Double
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## Parameters 

`amplitude`  

The input vector that defines the amplitude values.

`decibels`  

The output vector that contains the decibel values.

`zeroReference`  

The zero reference that the function uses for the conversion.

## Discussion

The function uses the following calculation to perform the conversion:

```
alpha = 20;

for (n = 0; n 

## See Also

### Converting double-precision power or amplitude values to decibel values

static func amplitudeToDecibels&lt;U>(U, zeroReference: Double) -> [Double]

Returns double-precision amplitude values converted to decibel values.

static func powerToDecibels&lt;U>(U, zeroReference: Double) -> [Double]

Returns double-precision power values converted to decibel values.

static func convert&lt;U, V>(power: U, toDecibels: inout V, zeroReference: Double)

Converts double-precision power values to decibel values.

