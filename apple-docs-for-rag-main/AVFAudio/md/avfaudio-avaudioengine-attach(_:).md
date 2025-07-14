

- AVFAudio
- AVAudioEngine
-  attach(\_:) 

Instance Method

# attach(\_:)

Attaches an audio node to the audio engine.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attach(_ node: AVAudioNode)
```

## Parameters 

`node`  

The audio node to attach.

## Discussion

An instance of AVAudioNode isn’t usable until you attach it to the audio engine using this method.

```
// Create a player node that's used for audio playback.
let playerNode = AVAudioPlayerNode()

// Attach the player node to the engine.
engine.attach(playerNode)
```

## See Also

### Attaching and Detaching Audio Nodes

func detach(AVAudioNode)

Detaches an audio node from the audio engine.

var attachedNodes: Set&lt;AVAudioNode>

A read-only set that contains the nodes you attach to the audio engine.

