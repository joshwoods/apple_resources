

- Model I/O
- MDLSkyCubeTexture
-  sunElevation 

Instance Property

# sunElevation

The sun’s position in the simulated sky.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sunElevation: Float { get set }
```

## Discussion

An elevation of `1.0` places the sun at the zenith (the center of the top face of the cube texture), a value of `0.0` places the sun at the nadir (the center of the bottom face), and a value of `0.5` places the sun on the horizon. The azimuth angle of the sun is fixed; to control the horizontal position of the sun relative to scene content, rotate the scene element responsible for displaying the sky cube texture.

Combine changes to this property with different turbidity and upperAtmosphereScattering to create sunset, dawn, or twilight effects.

## See Also

### Working with Sky Simulation Parameters

var turbidity: Float

The cloudiness or haziness of the simulated sky.

var upperAtmosphereScattering: Float

A factor that influences the color of the simulated sky.

var groundAlbedo: Float

A factor that influences the clarity of the simulated sky.

var groundColor: CGColor?

The color of the simulated ground.

var horizonElevation: Float

The angle, in radians relative to center, below which to render the ground color.

