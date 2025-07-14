

- SceneKit
- SCNAudioPlayer
-  didFinishPlayback 

Instance Property

# didFinishPlayback

A block called by SceneKit when playback of the player’s audio source has completed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var didFinishPlayback: (() -> Void)? { get set }
```

## Discussion

The block takes no parameters and returns no value. Use this block to perform actions when a sound finishes playing. For example, after a line of spoken character dialogue finishes playing, you might start playing another line of dialogue.

## See Also

### Responding to Playback

var willStartPlayback: (() -> Void)?

A block called by SceneKit when playback of the player’s audio source is about to begin.

