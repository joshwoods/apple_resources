

- Metal
- MTLRasterizationRateMap
-  physicalSize(layer:) 

Instance Method

# physicalSize(layer:)

Returns the dimensions, in pixels, of the area in the render target affected by the rasterization rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func physicalSize(layer layerIndex: Int) -> MTLSize
```

**Required**

## Parameters 

`layerIndex`  

The index of the layer.

## Return Value

The dimensions, in pixels, of the area in the render target affected by the rasterization rate map.

## Mentioned in 

Rendering with a Rasterization Rate Map

## Discussion

Your render targets should be at least as large as the physical size returned by this method. Each layer may have different rasterization rates and therefore different physical size requirements.

## See Also

### Inspecting Geometric and Rendering Properties

var layerCount: Int

The number of layers in the rate map.

**Required**

var screenSize: MTLSize

The logical size, in pixels, of the viewport coordinate system.

**Required**

var physicalGranularity: MTLSize

The granularity, in physical pixels, at which the rasterization rate varies.

**Required**

