

- AVFoundation
- AVVideoCompositionInstructionProtocol
-  containsTweening 

Instance Property

# containsTweening

A Boolean value that indicates whether the composition contains tweening.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var containsTweening: Bool { get }
```

**Required**

## Discussion

A value of true indicates that rendering a frame from the same source buffers and the same composition instruction at two different compositionTime values may yield different output frames. A value of false indicates that two compositions yield the same frame.

