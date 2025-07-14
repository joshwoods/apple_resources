

- Metal
- MTLSharedTextureHandle
-  device 

Instance Property

# device

The device object that created the texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

## Discussion

A texture is always associated with the MTLDevice that created it and can be used only with that device.

## See Also

### Identifying the Shared Texture Handle

var label: String?

A string that identifies the texture.

