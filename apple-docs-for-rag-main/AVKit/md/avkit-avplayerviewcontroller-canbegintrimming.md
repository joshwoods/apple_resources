

- AVKit
- AVPlayerViewController
-  canBeginTrimming 

Instance Property

# canBeginTrimming

A Boolean value that indicates whether the current media supports trimming.

visionOS 1.0+

``` source
@MainActor
var canBeginTrimming: Bool { get }
```

## Mentioned in 

Trimming and exporting media in visionOS

## Discussion

Not all media supports trimming. For example, this property returns false for HTTP Live Streaming media or protected content.

Observe this property to determine when to change the enabled state of your app UI that initiates trimming.

## See Also

### Presenting the visionOS Trimming UI

func beginTrimming(completionHandler: ((Bool) -> Void)?)

Presents the system trimming interface controls inside the player view.

