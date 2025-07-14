

- Accelerate
- vDSP
-  convert(power:toDecibels:zeroReference:) 

Type Method

# convert(power:toDecibels:zeroReference:)

Converts single-precision power values to decibel values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convert(
    power: U,
    toDecibels decibels: inout V,
    zeroReference: Float
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## Parameters 

`power`  

The input vector that defines the power values.

`decibels`  

The output vector that contains the decibel values.

`zeroReference`  

The zero reference that the function uses for the conversion.

## Discussion

The function uses the following calculation to perform the conversion:

```
alpha = 10;

for (n = 0; n 

## See Also

### Converting single-precision power or amplitude values to decibel values

static func amplitudeToDecibels&lt;U>(U, zeroReference: Float) -> [Float]

Returns single-precision amplitude values converted to decibels.

static func powerToDecibels&lt;U>(U, zeroReference: Float) -> [Float]

Returns single-precision power values converted to decibel values.

static func convert&lt;U, V>(amplitude: U, toDecibels: inout V, zeroReference: Float)

Converts single-precision amplitude values to decibel values.

