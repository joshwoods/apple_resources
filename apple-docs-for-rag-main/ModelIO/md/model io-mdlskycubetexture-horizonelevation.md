

- Model I/O
- MDLSkyCubeTexture
-  horizonElevation 

Instance Property

# horizonElevation

The angle, in radians relative to center, below which to render the ground color.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var horizonElevation: Float { get set }
```

## Discussion

By default, Model I/O renders an infinite sky above and below. If you set the groundColor property, Model I/O renders a solid color for all areas of the cube texture below this elevation. An elevation of `0.0` renders a horizon at the center elevation of the sky cube; negative values lead to a lower horizon and positive values to a higher horizon.

## See Also

### Working with Sky Simulation Parameters

var turbidity: Float

The cloudiness or haziness of the simulated sky.

var sunElevation: Float

The sun’s position in the simulated sky.

var upperAtmosphereScattering: Float

A factor that influences the color of the simulated sky.

var groundAlbedo: Float

A factor that influences the clarity of the simulated sky.

var groundColor: CGColor?

The color of the simulated ground.

