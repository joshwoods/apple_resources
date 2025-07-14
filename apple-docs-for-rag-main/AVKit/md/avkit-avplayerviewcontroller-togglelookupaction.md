

- AVKit
- AVPlayerViewController
-  toggleLookupAction 

Instance Property

# toggleLookupAction

An action that enables the visual lookup interface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+

``` source
@MainActor
var toggleLookupAction: UIAction { get }
```

## Discussion

When a user toggles the lookup UI, the state property is UIMenuElement.State.on, and is UIMenuElement.State.off otherwise. The system disables the action’s attributes when there isn’t visual lookup data available or when the media is playing.

## See Also

### Configuring Frame Analysis

var allowsVideoFrameAnalysis: Bool

A Boolean value that indicates whether to perform video frame analysis.

var videoFrameAnalysisTypes: AVVideoFrameAnalysisType

The types of analysis a player view controller performs on a paused video frame.

struct AVVideoFrameAnalysisType

Constants that define the types of analysis a player view controller may perform on a paused video frame.

