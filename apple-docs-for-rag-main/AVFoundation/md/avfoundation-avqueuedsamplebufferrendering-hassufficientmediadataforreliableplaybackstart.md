

- AVFoundation
- AVQueuedSampleBufferRendering
-  hasSufficientMediaDataForReliablePlaybackStart 

Instance Property

# hasSufficientMediaDataForReliablePlaybackStart

A Boolean value that indicates whether the enqued media meets the required preroll level for reliable playback.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
var hasSufficientMediaDataForReliablePlaybackStart: Bool { get }
```

**Required**

## Discussion

Starting playback when this property is false may prevent smooth playback following an immediate start.

