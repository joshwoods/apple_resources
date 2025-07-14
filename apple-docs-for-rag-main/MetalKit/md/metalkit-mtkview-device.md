

- MetalKit
- MTKView
-  device 

Instance Property

# device

The device object the view uses to create its Metal objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var device: (any MTLDevice)? { get set }
```

## Discussion

The default value is `nil`. You must explicitly set the device object.

## See Also

### Configuring the Metal Device

var preferredDevice: (any MTLDevice)?

The device object that the system recommends using for this view.

