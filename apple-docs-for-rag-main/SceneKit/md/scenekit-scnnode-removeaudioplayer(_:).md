

- SceneKit
- SCNNode
-  removeAudioPlayer(\_:) 

Instance Method

# removeAudioPlayer(\_:)

Removes the specified audio player from the node, stopping playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeAudioPlayer(_ player: SCNAudioPlayer)
```

## Parameters 

`player`  

An audio player attached to the node.

## Discussion

This method has no effect if the `player` parameter does not reference an audio player directly attached to the node.

## See Also

### Working with Positional Audio

func addAudioPlayer(SCNAudioPlayer)

Adds the specified auto player to the node and begins playback.

var audioPlayers: [SCNAudioPlayer]

The audio players currently attached to the node.

func removeAllAudioPlayers()

Removes all audio players attached to the node, stopping playback.

