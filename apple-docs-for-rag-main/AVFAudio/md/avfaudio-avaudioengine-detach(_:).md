

- AVFAudio
- AVAudioEngine
-  detach(\_:) 

Instance Method

# detach(\_:)

Detaches an audio node from the audio engine.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func detach(_ node: AVAudioNode)
```

## Parameters 

`node`  

The audio node to detach.

## Discussion

If necessary, the audio engine safely disconnects the audio node before detaching it.

## See Also

### Attaching and Detaching Audio Nodes

func attach(AVAudioNode)

Attaches an audio node to the audio engine.

var attachedNodes: Set&lt;AVAudioNode>

A read-only set that contains the nodes you attach to the audio engine.

