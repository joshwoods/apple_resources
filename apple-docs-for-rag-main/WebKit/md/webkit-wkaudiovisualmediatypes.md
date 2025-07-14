

- WebKit
-  WKAudiovisualMediaTypes 

Structure

# WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
struct WKAudiovisualMediaTypes
```

## Overview

To indicate that no user gestures are required to play media, use an empty set of audio/visual media types, indicated by the empty array literal, `[]`. For example, `let myAudiovisualMediaType: WKAudiovisualMediaTypes = []`.

## Topics

### Media Types

static var audio: WKAudiovisualMediaTypes

Media types that contain audio require a user gesture to begin playing.

static var video: WKAudiovisualMediaTypes

Media types that contain video require a user gesture to begin playing.

static var all: WKAudiovisualMediaTypes

All media types require a user gesture to begin playing.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting media playback preferences

var allowsInlineMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos play inline or use the native full-screen controller.

var allowsAirPlayForMediaPlayback: Bool

A Boolean value that indicates whether the web view allows media playback over AirPlay.

var allowsPictureInPictureMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos can play Picture in Picture.

var mediaTypesRequiringUserActionForPlayback: WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

