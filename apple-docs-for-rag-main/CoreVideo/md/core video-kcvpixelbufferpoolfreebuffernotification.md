

- Core Video
-  kCVPixelBufferPoolFreeBufferNotification 

Global Variable

# kCVPixelBufferPoolFreeBufferNotification

A notification that the system posts if a buffer becomes available after it fails to create a pixel buffer with auxiliary attributes because it exceeded the threshold you specified.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCVPixelBufferPoolFreeBufferNotification: CFString
```

## Discussion

The system posts this notification if a buffer becomes available after the CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(_:_:_:_:) function fails because the system exceeds the threshold you set for the kCVPixelBufferPoolAllocationThresholdKey key. The system won’t post this notification if you don’t set a value for the kCVPixelBufferPoolAllocationThresholdKey key for the `auxAttributes` parameter of the CVPixelBufferPoolCreatePixelBufferWithAuxAttributes(_:_:_:_:) function.

