

- Model I/O
- MDLSkyCubeTexture
-  upperAtmosphereScattering 

Instance Property

# upperAtmosphereScattering

A factor that influences the color of the simulated sky.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var upperAtmosphereScattering: Float { get set }
```

## Discussion

This value affects the intensity of sunlight and the color of the sky. A value of `0.0` produces muted, dusky colors, and a value of 1.0 produces saturated, noon-like sky colors.

## See Also

### Working with Sky Simulation Parameters

var turbidity: Float

The cloudiness or haziness of the simulated sky.

var sunElevation: Float

The sun’s position in the simulated sky.

var groundAlbedo: Float

A factor that influences the clarity of the simulated sky.

var groundColor: CGColor?

The color of the simulated ground.

var horizonElevation: Float

The angle, in radians relative to center, below which to render the ground color.

