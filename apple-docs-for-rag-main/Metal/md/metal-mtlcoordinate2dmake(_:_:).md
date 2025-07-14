

- Metal
-  MTLCoordinate2DMake(\_:\_:) 

Function

# MTLCoordinate2DMake(\_:\_:)

Returns a new 2D point with the specified coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLCoordinate2DMake(
    _ x: Float,
    _ y: Float
) -> MTLCoordinate2D
```

## Parameters 

`x`  

The x coordinate of the new point.

`y`  

The y coordinate of the new point.

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

typealias MTLCoordinate2D

A coordinate in the viewport.

