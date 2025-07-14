

- Metal
- MTLRasterizationRateMapDescriptor
-  init(screenSize:layer:label:) 

Initializer

# init(screenSize:layer:label:)

A convenience initializer that creates a rate map descriptor with a single rate layer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS

``` source
convenience init(
    screenSize: MTLSize,
    layer: MTLRasterizationRateLayerDescriptor,
    label: String? = nil
)
```

## Parameters 

`screenSize`  

The logical size, in pixels, of the viewport coordinate system.

`layer`  

A descriptor for the rate layer to create.

`label`  

A string that identifies the resulting rate map.

## Return Value

A descriptor object whose screenSize and label properties are set to the provided values. Layer `0` in the rate map is set to the provided layer descriptor.

## See Also

### Creating Rate Map Descriptors

convenience init(screenSize: MTLSize, label: String?)

A convenience initializer that creates a rate map descriptor with a given size and identifier.

convenience init(screenSize: MTLSize, layers: [MTLRasterizationRateLayerDescriptor], label: String?)

A convenience initializer that creates a rate map descriptor with a set of layer descriptors.

