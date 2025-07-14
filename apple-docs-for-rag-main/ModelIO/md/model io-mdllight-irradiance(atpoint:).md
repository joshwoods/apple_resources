

- Model I/O
- MDLLight
-  irradiance(atPoint:) 

Instance Method

# irradiance(atPoint:)

Returns the radiance of the light as received at a specific point in the same scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func irradiance(atPoint point: vector_float3) -> Unmanaged
```

## Parameters 

`point`  

A point in the same world coordinate space as the light.

## Return Value

The color and intensity of the light’s effect on the specified point.

## Discussion

Calling this method is equivalent to calling the irradiance(atPoint:colorSpace:) method and passing the Rec. 709 color space. (See `kCGColorSpaceITUR_709`.)

## See Also

### Working with Lights

func irradiance(atPoint: vector_float3, colorSpace: CGColorSpace) -> Unmanaged&lt;CGColor>

Returns the radiance of the light as received at a specific point in the same scene, expressed using the specified color space.

var lightType: MDLLightType

The type of the light.

var colorSpace: String

The name of the Core Graphics color space to be used for interpreting the light’s color information.

