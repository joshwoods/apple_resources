

- SceneKit
- SCNAudioPlayer
-  init(source:) 

Initializer

# init(source:)

Initializes an audio player for playing the specified simple audio source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(source: SCNAudioSource)
```

## Parameters 

`source`  

An audio source object.

## Return Value

A positional audio player object.

## Discussion

Using this initializer is typically not necessary. Instead, call the audioPlayerWithSource: method, which returns a cached audio player object if one for the specified audio source has already been created and is available for use.

## See Also

### Creating an Audio Player

init(avAudioNode: AVAudioNode)

Initializes an audio player for playing the specified AVFoundation audio node.

