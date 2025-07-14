

- SceneKit
-  SCNAudioPlayer 

Class

# SCNAudioPlayer

A controller for playback of a positional audio source in a SceneKit scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class SCNAudioPlayer
```

## Overview

An SCNAudioPlayer object controls playback of a positional audio source in a SceneKit scene. To use positional audio, first create a reusable SCNAudioSource or AVAudioNode object to provide an audio stream. Then, create an audio player to control the playback of that audio source. Finally, attach the audio player to an SCNNode object for spatialized 3D audio playback based on the position of that node relative to the scene’s audioListener node.

## Topics

### Creating an Audio Player

init(source: SCNAudioSource)

Initializes an audio player for playing the specified simple audio source.

init(avAudioNode: AVAudioNode)

Initializes an audio player for playing the specified AVFoundation audio node.

### Working with Audio Sources

var audioSource: SCNAudioSource?

The source of audio played by this player.

var audioNode: AVAudioNode?

The audio node SceneKit uses for mixing audio from this player.

### Responding to Playback

var willStartPlayback: (() -> Void)?

A block called by SceneKit when playback of the player’s audio source is about to begin.

var didFinishPlayback: (() -> Void)?

A block called by SceneKit when playback of the player’s audio source has completed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio

class SCNAudioSource

A simple, reusable audio source—music or sound effects loaded from a file—for use in positional audio playback.

