

- RealityKit
-  VideoPlaybackController 

Class

# VideoPlaybackController

An object that controls the playback of video for a video material.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
@MainActor @preconcurrency
class VideoPlaybackController
```

## Topics

### Instance Properties

var audioInputMode: AudioResource.InputModeDeprecated

var currentImageSize: CGSize?

What is the width and height of currently playing video (for stereo, the width and height of each eye)? This is optional because the video may not currently be playing, or the size is otherwise not available.

var currentViewingMode: VideoPlaybackController.ViewingMode?

Is the currently playing video in mono or stereo? This is optional because the video may not currently be playing, or the mode is otherwise not available.

var preferredViewingMode: VideoPlaybackController.ViewingMode

Do we want to play stereo video in mono or stereo? Default is to play in stereo.

var reverbSendLevel: AudioPlaybackController.DecibelDeprecated

### Enumerations

enum ViewingMode

Options for viewing video playback.

## Relationships

### Conforms To

- Sendable

## See Also

### Video player configurations

struct VideoPlayerComponent

A component that supports general video-playback experience with an AV player.

enum ImmersiveViewingMode

Options for viewing the video during immersive-media playback.

struct VideoMaterial

A material that supports animated textures.

enum ViewingMode

Options for viewing video playback.

