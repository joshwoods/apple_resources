

- Video Toolbox
- VTRAWProcessingSession
-  metalDevice 

Instance Property

# metalDevice

The preferred device to use for any Metal-based processing performed by the RAW Processing Extension.

macOS 15.0+

``` source
var metalDevice: (any MTLDevice)? { get set }
```

## Discussion

Setting a value of `nil` indicates that the client has no preferred Metal device. Getting `nil` indicates that no preferred device was set or that the processor does not use Metal for frame processing.

