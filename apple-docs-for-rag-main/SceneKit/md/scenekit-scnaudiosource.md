

- SceneKit
-  SCNAudioSource 

Class

# SCNAudioSource

A simple, reusable audio source—music or sound effects loaded from a file—for use in positional audio playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class SCNAudioSource
```

## Overview

To create positional audio effects, create an SCNAudioPlayer object from the audio source to control playback, and add that player object to an SCNNode object in your scene. SceneKit then automatically spatializes 3D audio effects based on the position of that node relative to the scene’s audioListener node.

## Topics

### Creating an Audio Source

convenience init?(named: String)

Returns the audio source associated with the specified filename.

convenience init?(fileNamed: String)

Initializes an audio source from an audio file in the application’s main bundle.

init?(url: URL)

Initializes an audio source from the specified audio file.

### Controlling 3D Audio Spatialization

var isPositional: Bool

A Boolean value that determines whether audio from this source uses 3D positional mixing.

### Preloading Audio Data

func load()

Loads audio data from the source and prepares it for playing.

### Setting Default Playback Parameters

var volume: Float

The default playback volume for the audio source.

var rate: Float

The default playback rate for the audio source.

var reverbBlend: Float

The default blend of blend of unmodified and reverb-processed (also called dry and wet) audio for playback of the audio source.

var loops: Bool

A Boolean value that determines whether the audio source should play repeatedly.

var shouldStream: Bool

A Boolean value that determines whether the audio source should stream content from its source URL when playing.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Audio

class SCNAudioPlayer

A controller for playback of a positional audio source in a SceneKit scene.

