

- ARKit
- ARDepthData
-  confidenceMap 

Instance Property

# confidenceMap

The framework’s confidence in the accuracy of the depth-map data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
unowned(unsafe) var confidenceMap: CVPixelBuffer? { get }
```

## Discussion

The natural light of the physical environment affects the depthMap property such that ARKit is less confident about the accuracy of the LiDAR Scanner’s depth measurements for surfaces that are highly reflective, or that have high light absorption. This property measures the accuracy of the scene depth-data by containing an ARConfidenceLevel raw-value for every component in depthMap.

Custom renderers that process confidence data on the GPU should choose a MTLPixelFormat according to the confidenceMap pixel format the app reads at runtime. Call CVPixelBufferGetPixelFormatType(_:) on the confidenceMap to get its format. If, for example, the confidenceMap format is kCVPixelFormatType_OneComponent8 (OSType \``L008`\`), create a Metal texture with format MTLPixelFormat.r8Uint to send confidence data to the GPU.

## See Also

### Depth Information

var depthMap: CVPixelBuffer

The estimated distance from the device to its environment, in meters.

enum ARConfidenceLevel

Degrees to which the framework is confident about depth-data accuracy.

