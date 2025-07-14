

- AVFoundation
-  AVVideoCompositionRenderHint 

Class

# AVVideoCompositionRenderHint

Information about upcoming composition requests, such as composition start time and end time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class AVVideoCompositionRenderHint
```

## Topics

### Managing Composition Timing

var startCompositionTime: CMTime

The start time of the upcoming composition requests.

var endCompositionTime: CMTime

The end time of the upcoming composition requests.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Preparing to Render Frames

func anticipateRendering(using: AVVideoCompositionRenderHint)

Informs a custom video compositor about upcoming rendering requests.

func prerollForRendering(using: AVVideoCompositionRenderHint)

Tells a custom video compositor to perform any work in the prerolling phase.

