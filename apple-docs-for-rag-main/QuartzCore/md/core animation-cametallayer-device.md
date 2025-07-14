

- Core Animation
- CAMetalLayer
-  device 

Instance Property

# device

The Metal device responsible for the layer’s drawable resources.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var device: (any MTLDevice)? { get set }
```

## Discussion

This property determines which device object Metal uses to create its MTLTexture objects. When you retrieve a drawable object and its associated texture, you must render to the texture using the same device object.

The default value is `nil`—you must set the device for a layer before rendering.

## See Also

### Related Documentation

Core Animation Programming Guide

Metal Programming Guide

### Configuring the Metal Device

var preferredDevice: (any MTLDevice)?

The device object that the system recommends using for this layer.

