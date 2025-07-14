

- Metal
-  MTLRasterizationRateMapDescriptor 

Class

# MTLRasterizationRateMapDescriptor

An object that you use to configure new rasterization rate maps.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
class MTLRasterizationRateMapDescriptor
```

## Overview

To create a new rate map, first create an MTLRasterizationRateMapDescriptor instance and set its property values. Then, create a new rasterization rate-map by calling an MTLDevice instance’s  
makeRasterizationRateMap(descriptor:) method.

When creating a rate map, Metal copies into it property values from the descriptor. You can reuse a descrptor by modifying its property values, which doesn’t affect the other rate-map instances that already exist.

## Topics

### Creating Rate Map Descriptors

convenience init(screenSize: MTLSize, label: String?)

A convenience initializer that creates a rate map descriptor with a given size and identifier.

convenience init(screenSize: MTLSize, layer: MTLRasterizationRateLayerDescriptor, label: String?)

A convenience initializer that creates a rate map descriptor with a single rate layer.

convenience init(screenSize: MTLSize, layers: [MTLRasterizationRateLayerDescriptor], label: String?)

A convenience initializer that creates a rate map descriptor with a set of layer descriptors.

### Identifying the Rate Map

var label: String?

A string used to identify the rate map you create with the descriptor.

### Configuring the Viewport Size

var screenSize: MTLSize

The size of the viewport coordinate system, in logical pixels.

### Configuring the Rate Map Layers

var layerCount: Int

The number of layers in the rate map.

func layer(at: Int) -> MTLRasterizationRateLayerDescriptor?

Returns the layer description for a layer in the rate map.

func setLayer(MTLRasterizationRateLayerDescriptor?, at: Int)

Sets a configuration for a layer rate map.

var layers: MTLRasterizationRateLayerArray

The rasterization rates for one or more layers in the rate map.

class MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

protocol MTLRasterizationRateMap

A compiled read-only object that determines how to apply variable rasterization rates when rendering.

typealias MTLCoordinate2D

A coordinate in the viewport.

func MTLCoordinate2DMake(Float, Float) -> MTLCoordinate2D

Returns a new 2D point with the specified coordinates.

