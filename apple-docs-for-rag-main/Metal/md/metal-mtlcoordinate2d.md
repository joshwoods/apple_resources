

- Metal
-  MTLCoordinate2D 

Type Alias

# MTLCoordinate2D

A coordinate in the viewport.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLCoordinate2D = MTLSamplePosition
```

## See Also

### Rasterization Settings

Rendering at Different Rasterization Rates

Configure a rasterization rate map to vary rasterization rates depending on the amount of detail needed.

Creating a Rasterization Rate Map

Define the rasterization rates for each part of your render target.

Rendering with a Rasterization Rate Map

Create offscreen textures to hold intermediate rasterized data.

Scaling Variable Rasterization Rate Content

Use the rate map data to scale the content to fill your destination texture.

class MTLRasterizationRateMapDescriptor

An object that you use to configure new rasterization rate maps.

protocol MTLRasterizationRateMap

A compiled read-only object that determines how to apply variable rasterization rates when rendering.

func MTLCoordinate2DMake(Float, Float) -> MTLCoordinate2D

Returns a new 2D point with the specified coordinates.

