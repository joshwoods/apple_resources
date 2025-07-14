

- Model I/O
- MDLLight
-  colorSpace 

Instance Property

# colorSpace

The name of the Core Graphics color space to be used for interpreting the light’s color information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var colorSpace: String { get set }
```

## See Also

### Working with Lights

func irradiance(atPoint: vector_float3) -> Unmanaged&lt;CGColor>

Returns the radiance of the light as received at a specific point in the same scene.

func irradiance(atPoint: vector_float3, colorSpace: CGColorSpace) -> Unmanaged&lt;CGColor>

Returns the radiance of the light as received at a specific point in the same scene, expressed using the specified color space.

var lightType: MDLLightType

The type of the light.

