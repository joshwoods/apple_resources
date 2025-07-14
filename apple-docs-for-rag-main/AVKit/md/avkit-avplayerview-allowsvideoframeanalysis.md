

- AVKit
- AVPlayerView
-  allowsVideoFrameAnalysis 

Instance Property

# allowsVideoFrameAnalysis

A Boolean value that indicates whether to perform video frame analysis.

macOS 13.0+

``` source
@MainActor
var allowsVideoFrameAnalysis: Bool { get set }
```

## Discussion

If the value is true, a player view tries to find objects, text, and people when you pause media playback. If it finds an object, the user is able to interact with it using a long press to present a context menu.

The default value is true.

## See Also

### Configuring Frame Analysis

var videoFrameAnalysisTypes: AVVideoFrameAnalysisType

struct AVVideoFrameAnalysisType

Constants that define the types of analysis a player view controller may perform on a paused video frame.

