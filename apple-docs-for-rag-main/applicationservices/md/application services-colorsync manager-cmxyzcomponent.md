

- Application Services
- ColorSync Manager
-  CMXYZComponent 

Type Alias

# CMXYZComponent

macOS 10.0+

``` source
typealias CMXYZComponent = UInt16
```

## Discussion

Three components combine to express a color value defined by the `CMXYZColor` type definition in the XYZ color space. Each color component is described by a numeric value defined by the `CMXYZComponent` type definition. A component value of type `CMXYZComponent` is expressed as a 16-bit value. This is formatted as an unsigned value with 1 bit of integer portion and 15 bits of fractional portion.

