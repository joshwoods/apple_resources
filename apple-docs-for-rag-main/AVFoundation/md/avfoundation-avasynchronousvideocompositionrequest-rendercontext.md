

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  renderContext 

Instance Property

# renderContext

The rendering context of the video composition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var renderContext: AVVideoCompositionRenderContext { get }
```

## See Also

### Inspecting the Request

var compositionTime: CMTime

A time for which to compose the frame.

var videoCompositionInstruction: any AVVideoCompositionInstructionProtocol

A video composition instruction that indicates how to compose the frame.

