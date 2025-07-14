

- SceneKit
- SCNNode
-  addAudioPlayer(\_:) 

Instance Method

# addAudioPlayer(\_:)

Adds the specified auto player to the node and begins playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addAudioPlayer(_ player: SCNAudioPlayer)
```

## Parameters 

`player`  

An audio player object.

## Discussion

Positional audio effects from a player attached to a node are based on that node’s position relative to the audioListener position in the scene.

After playback has completed, SceneKit automatically removes the audio player from the node.

## See Also

### Working with Positional Audio

var audioPlayers: [SCNAudioPlayer]

The audio players currently attached to the node.

func removeAudioPlayer(SCNAudioPlayer)

Removes the specified audio player from the node, stopping playback.

func removeAllAudioPlayers()

Removes all audio players attached to the node, stopping playback.

