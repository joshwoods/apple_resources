

- PHASE
- PHASECardioidDirectivityModelSubbandParameters
-  sharpness 

Instance Property

# sharpness

The amount that the shape overlaps with bordering subbands.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var sharpness: Double { get set }
```

## Discussion

This property condenses the shape of the pattern such that higher values extend the shape frontwards. Increasing sharpness for dipole (a pattern value of `1.0`), extends the shape frontwards and backwards.

The default value is `1.0`. Values greater than `1.0` increase sharpness. The framework clamps the value to the range `[1.0,` greatestFiniteMagnitude`]`.

## See Also

### Shaping Directivity

var pattern: Double

A shape that determines the direction of sound.

