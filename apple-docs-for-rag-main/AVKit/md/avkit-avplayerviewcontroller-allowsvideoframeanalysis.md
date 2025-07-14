

- AVKit
- AVPlayerViewController
-  allowsVideoFrameAnalysis 

Instance Property

# allowsVideoFrameAnalysis

A Boolean value that indicates whether to perform video frame analysis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 18.0+

``` source
@MainActor
var allowsVideoFrameAnalysis: Bool { get set }
```

## Discussion

If the value is true, a player view controller tries to find objects, text, and people when you pause media playback. If it finds an object, the user is able to interact with it using a long press to present a context menu.

The default value is true.

## See Also

### Configuring Frame Analysis

var toggleLookupAction: UIAction

An action that enables the visual lookup interface.

var videoFrameAnalysisTypes: AVVideoFrameAnalysisType

The types of analysis a player view controller performs on a paused video frame.

struct AVVideoFrameAnalysisType

Constants that define the types of analysis a player view controller may perform on a paused video frame.

