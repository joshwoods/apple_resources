

- AVFoundation
- Media playback
- AVPlayerItem
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Accessing Metadata

var timedMetadata: [AVMetadataItem]?

An array of the most recently encountered timed metadata.

Deprecated

### Seeking Through Media

func seek(to: CMTime)

Sets the current playback time to the specified time.

Deprecated

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime)

Sets the current playback time within a specified time bound.

Deprecated

func seek(to: Date) async -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

func seek(to: Date) -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

### Selecting Media Options

func selectedMediaOption(in: AVMediaSelectionGroup) -> AVMediaSelectionOption?

Returns the media selection option that’s currently selected from the specified group.

Deprecated

