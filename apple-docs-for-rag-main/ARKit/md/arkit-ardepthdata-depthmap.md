

- ARKit
- ARDepthData
-  depthMap 

Instance Property

# depthMap

The estimated distance from the device to its environment, in meters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
unowned(unsafe) var depthMap: CVPixelBuffer { get }
```

## Discussion

For custom renderers, if you create a texture to send depth data to the GPU, choose a MTLPixelFormat according to the depthMap pixel format. Call CVPixelBufferGetPixelFormatType(_:) on the depthMap to get its format. For example, if at runtime the depthMap format is kCVPixelFormatType_DepthFloat32 (OSType \``fdep`\`), use MTLPixelFormat.r32Float.

## See Also

### Depth Information

var confidenceMap: CVPixelBuffer?

The framework’s confidence in the accuracy of the depth-map data.

enum ARConfidenceLevel

Degrees to which the framework is confident about depth-data accuracy.

