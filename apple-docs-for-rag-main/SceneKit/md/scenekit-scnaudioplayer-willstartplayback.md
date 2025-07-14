

- SceneKit
- SCNAudioPlayer
-  willStartPlayback 

Instance Property

# willStartPlayback

A block called by SceneKit when playback of the player’s audio source is about to begin.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var willStartPlayback: (() -> Void)? { get set }
```

## Discussion

The block takes no parameters and returns no value. Use this block to perform actions in response to the playing of sounds.

## See Also

### Responding to Playback

var didFinishPlayback: (() -> Void)?

A block called by SceneKit when playback of the player’s audio source has completed.

