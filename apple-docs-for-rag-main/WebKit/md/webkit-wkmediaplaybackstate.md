

- WebKit
-  WKMediaPlaybackState 

Enumeration

# WKMediaPlaybackState

An enumeration that describes whether an audio or video presentation is playing, paused, or suspended.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
enum WKMediaPlaybackState
```

## Topics

### Constants

case none

There is no media to play back.

case paused

The media playback is paused.

case playing

The media is playing.

case suspended

The media is not playing, and cannot be resumed until the user revokes the suspension.

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

### Interacting with media

func pauseAllMediaPlayback(completionHandler: (() -> Void)?)

Pauses playback of all media in the web view.

func requestMediaPlaybackState(completionHandler: (WKMediaPlaybackState) -> Void)

Requests the playback status of media in the web view.

func setAllMediaPlaybackSuspended(Bool, completionHandler: (() -> Void)?)

Changes whether the webpage is suspending playback of all media in the page.

func closeAllMediaPresentations(completionHandler: (() -> Void)?)

Closes all media the web view is presenting, including picture-in-picture video and fullscreen video.

