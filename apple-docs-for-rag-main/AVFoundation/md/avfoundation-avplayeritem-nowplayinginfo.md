

- AVFoundation
- AVPlayerItem
-  nowPlayingInfo 

Instance Property

# nowPlayingInfo

The current now playing information for the player item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var nowPlayingInfo: [String : Any]? { get set }
```

## Discussion

Setting this value to `nil` clears the player item’s now playing information.

