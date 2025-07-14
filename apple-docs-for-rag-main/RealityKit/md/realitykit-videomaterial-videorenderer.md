

- RealityKit
- VideoMaterial
-  videoRenderer 

Instance Property

# videoRenderer

The material’s video renderer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var videoRenderer: AVSampleBufferVideoRenderer? { get }
```

## Discussion

Pass this renderer to the material as a parameter in the initializer; you can’t replace it afterward. You can’t use the same `AVSampleBufferVideoRenderer` object with more than one `VideoMaterial`.

