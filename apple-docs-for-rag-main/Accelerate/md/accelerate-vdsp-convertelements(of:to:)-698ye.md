

- Accelerate
- vDSP
-  convertElements(of:to:) 

Type Method

# convertElements(of:to:)

Converts double-precision values to single-precision values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convertElements(
    of source: U,
    to destination: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Float
```

## Parameters 

`source`  

The source vector.

`destination`  

On output, the source values converted to single-precision values.

## See Also

### Conversion between floating-point types

static func doubleToFloat&lt;U>(U) -> [Float]

Returns single-precision values converted from a double-precision source.

static func floatToDouble&lt;U>(U) -> [Double]

Returns double-precision values converted from a single-precision source.

static func convertElements&lt;U, V>(of: U, to: inout V)

Converts single-precision values to double-precision values.

