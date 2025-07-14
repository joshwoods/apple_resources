

- Vision
- StatefulRequest
-  minimumLatencyFrameCount 

Instance Property

# minimumLatencyFrameCount

The minimum number of frames that the request has to process before reporting any observations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var minimumLatencyFrameCount: Int { get }
```

**Required** Default implementation provided.

## Discussion

The request provides this information after it’s initialized with its required parameters.

Video-based requests often need a minimum number of frames before they can report any observations. For example, for movement detection that requires at least `5` frames, the minimumLatencyFrameCount for the request reports `5`, and after the request processes `5` frames, an observation returns the results.

## Default Implementations

### StatefulRequest Implementations

var minimumLatencyFrameCount: Int

## See Also

### Inspecting the request

var frameAnalysisSpacing: CMTime

The reciprocal of the maximum rate to process buffers.

**Required**

