

- Model I/O
- MDLSkyCubeTexture
-  groundAlbedo 

Instance Property

# groundAlbedo

A factor that influences the clarity of the simulated sky.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var groundAlbedo: Float { get set }
```

## Discussion

This value simulates the amount of light that bounces back up into the sky from the ground. A value of `0.0` produces a clear sky, and values closer to `10` reduce the contrast of the sky, producing a foggy effect.

## See Also

### Working with Sky Simulation Parameters

var turbidity: Float

The cloudiness or haziness of the simulated sky.

var sunElevation: Float

The sun’s position in the simulated sky.

var upperAtmosphereScattering: Float

A factor that influences the color of the simulated sky.

var groundColor: CGColor?

The color of the simulated ground.

var horizonElevation: Float

The angle, in radians relative to center, below which to render the ground color.

