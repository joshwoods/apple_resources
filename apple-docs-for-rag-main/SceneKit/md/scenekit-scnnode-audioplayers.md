

- SceneKit
- SCNNode
-  audioPlayers 

Instance Property

# audioPlayers

The audio players currently attached to the node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var audioPlayers: [SCNAudioPlayer] { get }
```

## Discussion

Positional audio effects from a player attached to a node are based on that node’s position relative to the audioListener position in the scene.

After an audio player completes playback, SceneKit automatically removes it from the node. Therefore, this array always contains audio players that are currently playing back audio.

## See Also

### Working with Positional Audio

func addAudioPlayer(SCNAudioPlayer)

Adds the specified auto player to the node and begins playback.

func removeAudioPlayer(SCNAudioPlayer)

Removes the specified audio player from the node, stopping playback.

func removeAllAudioPlayers()

Removes all audio players attached to the node, stopping playback.

