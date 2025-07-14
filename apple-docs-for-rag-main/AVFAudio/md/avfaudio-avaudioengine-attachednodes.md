

- AVFAudio
- AVAudioEngine
-  attachedNodes 

Instance Property

# attachedNodes

A read-only set that contains the nodes you attach to the audio engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var attachedNodes: Set { get }
```

## See Also

### Attaching and Detaching Audio Nodes

func attach(AVAudioNode)

Attaches an audio node to the audio engine.

func detach(AVAudioNode)

Detaches an audio node from the audio engine.

