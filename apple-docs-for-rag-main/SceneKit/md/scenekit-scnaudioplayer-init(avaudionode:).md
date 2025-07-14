

- SceneKit
- SCNAudioPlayer
-  init(avAudioNode:) 

Initializer

# init(avAudioNode:)

Initializes an audio player for playing the specified AVFoundation audio node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(avAudioNode audioNode: AVAudioNode)
```

## Parameters 

`audioNode`  

An audio node object.

## Return Value

A positional audio player object.

## Discussion

Using this initializer is typically not necessary. Instead, call the audioPlayerWithAVAudioNode: method, which returns a cached audio player object if one for the specified AVAudioNode object has already been created and is available for use.

## See Also

### Creating an Audio Player

init(source: SCNAudioSource)

Initializes an audio player for playing the specified simple audio source.

