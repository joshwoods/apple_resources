

- RealityKit
- VideoPlaybackController
-  VideoPlaybackController.ViewingMode 

Enumeration

# VideoPlaybackController.ViewingMode

Options for viewing video playback.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum ViewingMode
```

## Topics

### Operators

static func == (VideoPlaybackController.ViewingMode, VideoPlaybackController.ViewingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case mono

A viewing mode that presents video in monoscopic mode.

case stereo

A viewing mode that presents video in stereoscopic mode, if it’s available.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Video player configurations

struct VideoPlayerComponent

A component that supports general video-playback experience with an AV player.

enum ImmersiveViewingMode

Options for viewing the video during immersive-media playback.

struct VideoMaterial

A material that supports animated textures.

class VideoPlaybackController

An object that controls the playback of video for a video material.

