

- Cinematic
- CNRenderingSession
-  CNRenderingSession.FrameAttributes 

Structure

# CNRenderingSession.FrameAttributes

Controls the focus distance and aperture of the rendering for the frames.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct FrameAttributes
```

## Topics

### Initializers

init?(sampleBuffer: CMSampleBuffer, sessionAttributes: CNRenderingSession.Attributes)

Creates a structure representing a Cinematic rendering session based a sample buffer and session attributes.

init?(timedMetadataGroup: AVTimedMetadataGroup, sessionAttributes: CNRenderingSession.Attributes)

Creates a structure representing a Cinematic rendering session based on meta group and session attributes.

### Instance Properties

var fNumber: Float

The f-stop value that inversely affects the aperture used to render the Cinematic image.

var focusDisparity: Float

Represents the focus plane at which the rendered image should be in focus.

