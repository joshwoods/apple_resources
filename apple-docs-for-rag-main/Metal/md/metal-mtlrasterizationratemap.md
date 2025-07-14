

- Metal
-  MTLRasterizationRateMap 

Protocol

# MTLRasterizationRateMap

A compiled read-only object that determines how to apply variable rasterization rates when rendering.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLRasterizationRateMap : NSObjectProtocol
```

## Mentioned in 

Rendering with a Rasterization Rate Map

## Overview

Use a rasterization rate map to reduce rendering quality in less-important or less-sampled regions of the render target, such as areas affected by blur effects or a far-away cascade of a shadow map.

By default, a render pass doesn’t have a rasterization rate map, and the viewport coordinate system maps exactly to physical pixels in the targeted textures. If you apply a rasterization rate map to a render pass, the viewport coordinate system becomes a logical coordinate system, and the rate map describes how to map logical coordinates to physical pixels in the render pass’s targets. You can specify different rasterization rates in different regions of the logical coordinate system. When you do, those logical units map to fewer physical pixels, which means you can use smaller render targets and render fewer pixels, saving both memory and processing time. For more information, see Rendering at Different Rasterization Rates.

Don’t implement this protocol yourself; instead, create a MTLRasterizationRateMapDescriptor object, configure it, and then call the makeRasterizationRateMap(descriptor:) on a device object.

To apply a rasterization rate map to a render pass, set the render pass descriptor’s rasterizationRateMap property.

### Configuring the Rate Map

A rasterization rate map specifies the size of the viewport coordinate space in logical units and one or more *layer maps*. A layer map partitions the viewport coordinate space into a 2D grid of cells and defines the rasterization rate for each cell. If you aren’t using layered rendering, provide a single layer map; otherwise, provide one layer map for each layer. For more information about layered rendering, see Rendering to Multiple Texture Slices in a Draw Command.

You can query the physical size requirements for each layer in the render pass by calling the physicalSize(layer:) method. Your render targets must be at least this large.

## Topics

### Identifying the Rate Map

var device: any MTLDevice

The device object that created the rate map.

**Required**

var label: String?

A string that identifies the rate map.

**Required**

### Inspecting Geometric and Rendering Properties

var layerCount: Int

The number of layers in the rate map.

**Required**

var screenSize: MTLSize

The logical size, in pixels, of the viewport coordinate system.

**Required**

func physicalSize(layer: Int) -> MTLSize

Returns the dimensions, in pixels, of the area in the render target affected by the rasterization rate map.

**Required**

var physicalGranularity: MTLSize

The granularity, in physical pixels, at which the rasterization rate varies.

**Required**

### Converting Between Viewport and Physical Coordinates

func physicalCoordinates(screenCoordinates: MTLCoordinate2D, layer: Int) -> MTLCoordinate2D

Converts a point in logical viewport coordinates to the corresponding physical coordinates in a render layer.

**Required**

func screenCoordinates(physicalCoordinates: MTLCoordinate2D, layer: Int) -> MTLCoordinate2D

Converts a point in physical coordinates inside a layer to its corresponding logical viewport coordinates.

**Required**

### Obtaining Coordinate Transformation Data

var parameterDataSizeAndAlign: MTLSizeAndAlign

The size and alignment requirements to contain the coordinate transformation information in this rate map.

**Required**

func copyParameterData(buffer: any MTLBuffer, offset: Int)

Copies the parameter data into the provided buffer.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

typealias MTLCoordinate2D

A coordinate in the viewport.

func MTLCoordinate2DMake(Float, Float) -> MTLCoordinate2D

Returns a new 2D point with the specified coordinates.

