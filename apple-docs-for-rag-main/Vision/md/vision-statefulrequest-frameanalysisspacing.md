

- Vision
- StatefulRequest
-  frameAnalysisSpacing 

Instance Property

# frameAnalysisSpacing

The reciprocal of the maximum rate to process buffers.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var frameAnalysisSpacing: CMTime { get }
```

**Required**

## Discussion

The request won’t process buffers that fall within the frameAnalysisSpacing since the previously performed analysis. The analysis isn’t done by wall time but by analysis of the time stamps of the sample buffers the request processes.

## See Also

### Inspecting the request

var minimumLatencyFrameCount: Int

The minimum number of frames that the request has to process before reporting any observations.

**Required** Default implementation provided.

