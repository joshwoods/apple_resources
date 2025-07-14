

- Model I/O
- MDLSkyCubeTexture
-  groundColor 

Instance Property

# groundColor

The color of the simulated ground.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var groundColor: CGColor? { get set }
```

## Discussion

By default, this property’s value is `nil`, causing Model I/O to render an infinite sky above and below. If you set this property to a color, Model I/O renders a solid color for all areas of the cube texture below the level specified in the horizonElevation property.

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

var horizonElevation: Float

The angle, in radians relative to center, below which to render the ground color.

