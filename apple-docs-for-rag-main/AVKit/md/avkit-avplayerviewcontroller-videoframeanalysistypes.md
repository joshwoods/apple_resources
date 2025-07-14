

- AVKit
- AVPlayerViewController
-  videoFrameAnalysisTypes 

Instance Property

# videoFrameAnalysisTypes

The types of analysis a player view controller performs on a paused video frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+

``` source
@MainActor
var videoFrameAnalysisTypes: AVVideoFrameAnalysisType { get set }
```

## See Also

### Configuring Frame Analysis

var allowsVideoFrameAnalysis: Bool

A Boolean value that indicates whether to perform video frame analysis.

var toggleLookupAction: UIAction

An action that enables the visual lookup interface.

struct AVVideoFrameAnalysisType

Constants that define the types of analysis a player view controller may perform on a paused video frame.

