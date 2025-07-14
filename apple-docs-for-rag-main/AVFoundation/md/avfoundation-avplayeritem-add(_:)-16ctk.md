

- AVFoundation
- AVPlayerItem
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified player item output object to the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
func add(_ output: AVPlayerItemOutput)
```

## Parameters 

`output`  

The player item output object to associate with the item.

## Discussion

When you add an AVPlayerItemOutput object to an item, the samples associated with that output object are processed according to the rules for mixing, composing, or excluding content that the AVPlayer object honors for the specific media type. For example, video media is composed according to the instructions provided by the player item’s video composition object and audio media is mixed according to the parameters of its audio mix object.

## See Also

### Related Documentation

var audioMix: AVAudioMix?

The audio mix parameters to be applied during playback.

var videoComposition: AVVideoComposition?

The video composition settings to be applied during playback.

### Managing Player Item Outputs

var outputs: [AVPlayerItemOutput]

An array of outputs associated with the player item.

func remove(AVPlayerItemOutput)

Removes the specified player item output object from the receiver.

