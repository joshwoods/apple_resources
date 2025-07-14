

- Accelerate
- vDSP
-  amplitudeToDecibels(\_:zeroReference:) 

Type Method

# amplitudeToDecibels(\_:zeroReference:)

Returns single-precision amplitude values converted to decibels.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func amplitudeToDecibels(
    _ amplitude: U,
    zeroReference: Float
) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`amplitude`  

The input vector that defines the amplitude values.

`zeroReference`  

The zero reference that the function uses for the conversion.

## Discussion

The function uses the following calculation to perform the conversion:

```
alpha = 20;

for (n = 0; n 

## See Also

### Converting single-precision power or amplitude values to decibel values

static func powerToDecibels&lt;U>(U, zeroReference: Float) -> [Float]

Returns single-precision power values converted to decibel values.

static func convert&lt;U, V>(amplitude: U, toDecibels: inout V, zeroReference: Float)

Converts single-precision amplitude values to decibel values.

static func convert&lt;U, V>(power: U, toDecibels: inout V, zeroReference: Float)

Converts single-precision power values to decibel values.

