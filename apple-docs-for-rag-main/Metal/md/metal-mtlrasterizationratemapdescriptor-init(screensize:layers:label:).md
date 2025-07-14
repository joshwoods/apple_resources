

- Metal
- MTLRasterizationRateMapDescriptor
-  init(screenSize:layers:label:) 

Initializer

# init(screenSize:layers:label:)

A convenience initializer that creates a rate map descriptor with a set of layer descriptors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS

``` source
convenience init(
    screenSize: MTLSize,
    layers: [MTLRasterizationRateLayerDescriptor],
    label: String? = nil
)
```

## Parameters 

`screenSize`  

The logical size, in pixels, of the viewport coordinate system.

`layers`  

An array of rate layer descriptors for the rate map’s layers.

`label`  

A string that identifies the resulting rate map.

## Return Value

A descriptor object whose screenSize and label properties are set to the provided values and whose rate map layers are set to the array you provided.

## See Also

### Creating Rate Map Descriptors

convenience init(screenSize: MTLSize, label: String?)

A convenience initializer that creates a rate map descriptor with a given size and identifier.

convenience init(screenSize: MTLSize, layer: MTLRasterizationRateLayerDescriptor, label: String?)

A convenience initializer that creates a rate map descriptor with a single rate layer.

