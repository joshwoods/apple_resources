

- AVFoundation
- AVPlayer
-  isClosedCaptionDisplayEnabled Deprecated

Instance Property

# isClosedCaptionDisplayEnabled

A Boolean value that indicates whether the player uses closed captioning.

iOS 4.0–11.0DeprecatediPadOS 4.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–11.0Deprecated

``` source
@MainActor
var isClosedCaptionDisplayEnabled: Bool { get set }
```

Deprecated

Let a player enable closed captions automatically according to user preferences by setting the value of the appliesMediaSelectionCriteriaAutomatically property to true.

## Discussion

The player displays closed captions in the following cases:

- Closed captions are present in the media and the value of `closedCaptionDisplayEnabled` is true, or

- A media selection option representing a stream of closed captions is selected in the legible media selection group.

Note

It’s strongly recommended that you don’t rely on this property to control the display of closed captions and instead use the media selection capabilities of AVPlayer and AVPlayerItem. The media selection API works equally well for displaying SDH subtitles as well as other kinds of content offering accessibility features. See select(_:in:) for more details.

