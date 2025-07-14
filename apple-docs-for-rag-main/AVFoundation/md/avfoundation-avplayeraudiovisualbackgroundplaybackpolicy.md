

- AVFoundation
-  AVPlayerAudiovisualBackgroundPlaybackPolicy 

Enumeration

# AVPlayerAudiovisualBackgroundPlaybackPolicy

Policies that describe playback behavior when an app transitions to the background while playing video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum AVPlayerAudiovisualBackgroundPlaybackPolicy
```

## Topics

### Policies

case automatic

The system decides whether playback continues.

case continuesIfPossible

The app continues playback, if possible.

case pauses

The app pauses playback.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Background Playback

var audiovisualBackgroundPlaybackPolicy: AVPlayerAudiovisualBackgroundPlaybackPolicy

A policy that determines how playback of audiovisual media continues when the app transitions to the background.

