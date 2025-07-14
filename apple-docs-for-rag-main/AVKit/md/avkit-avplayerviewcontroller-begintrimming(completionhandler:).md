

- AVKit
- AVPlayerViewController
-  beginTrimming(completionHandler:) 

Instance Method

# beginTrimming(completionHandler:)

Presents the system trimming interface controls inside the player view.

visionOS 1.0+

``` source
@MainActor
func beginTrimming(completionHandler handler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func beginTrimming() async -> Bool
```

## Parameters 

`handler`  

A completion handler that the system calls with a Boolean value that indicates whether the user completed the trim operation, or if they canceled it.

## Mentioned in 

Trimming and exporting media in visionOS

## Discussion

After trimming is complete, you can access the trimmed range by querying the forwardPlaybackEndTime and reversePlaybackEndTime properties on the AVPlayerItem.

For more information on supporting trimming in your app, see Trimming and exporting media in visionOS.

## See Also

### Presenting the visionOS Trimming UI

var canBeginTrimming: Bool

A Boolean value that indicates whether the current media supports trimming.

