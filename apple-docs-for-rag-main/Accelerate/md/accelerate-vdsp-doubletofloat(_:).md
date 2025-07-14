

- Accelerate
- vDSP
-  doubleToFloat(\_:) 

Type Method

# doubleToFloat(\_:)

Returns single-precision values converted from a double-precision source.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func doubleToFloat(_ source: U) -> [Float] where U : AccelerateBuffer, U.Element == Double
```

## Parameters 

`source`  

The source vector.

## See Also

### Conversion between floating-point types

static func floatToDouble&lt;U>(U) -> [Double]

Returns double-precision values converted from a single-precision source.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts single-precision values to double-precision values.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts double-precision values to single-precision values.

