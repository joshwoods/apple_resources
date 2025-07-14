

- PHASE
- PHASECardioidDirectivityModelSubbandParameters
-  pattern 

Instance Property

# pattern

A shape that determines the direction of sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var pattern: Double { get set }
```

## Discussion

The framework clamps the value to the range `[0.0, 1.0]`. The default value is `0.0`, which creates an omnidirectional shape. The value `0.5` creates a cardioid shape. The value `1.0` creates a dipole shape.

## See Also

### Shaping Directivity

var sharpness: Double

The amount that the shape overlaps with bordering subbands.

