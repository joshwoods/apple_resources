

- Core Animation
- CAMetalLayer
-  preferredDevice 

Instance Property

# preferredDevice

The device object that the system recommends using for this layer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var preferredDevice: (any MTLDevice)? { get }
```

## Discussion

On systems with a single GPU, this method returns the default device object; see MTLCreateSystemDefaultDevice(). On systems with more than one GPU, this method returns the MTLDevice that was last used to composite and present the CAMetalLayer. This device object usually corresponds to the GPU associated with the screen that’s displaying the layer. If you set the layer’s device property to this device object, you reduce the number of cross-GPU texture copies that Core Animation must perform to present the layer’s contents onscreen.

## See Also

### Configuring the Metal Device

var device: (any MTLDevice)?

The Metal device responsible for the layer’s drawable resources.

