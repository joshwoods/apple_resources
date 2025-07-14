

- AVFoundation
-  AVMutableCompositionTrack 

Class

# AVMutableCompositionTrack

A mutable track in a composition that you use to insert, remove, and scale track segments without affecting their low-level representation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMutableCompositionTrack
```

## Overview

Use this object to define constraints for the temporal arrangement of the track segments. If you set the composition’s track segments, you can test whether they meet the constraints by calling the validateSegments(_:) method.

## Topics

### Configuring Track Properties

var isEnabled: Bool

A Boolean value that indicates whether the tracks is in an enabled state.

var naturalTimeScale: CMTimeScale

The time scale in which you can perform time-based operations without extra numerical conversion.

var languageCode: String?

The language associated with the track, as an ISO 639-2/T language code.

var extendedLanguageTag: String?

The language tag associated with the track, as an RFC 4646 language tag.

var preferredTransform: CGAffineTransform

The preferred transformation of the visual media data for display purposes.

var preferredVolume: Float

The volume the track prefers for its audible media data.

### Managing Time Ranges

var segments: [AVCompositionTrackSegment]!

The track segments that a composition track contains.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within the track.

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime) throws

Inserts a time range of media from a source track into a composition track.

func insertTimeRanges([NSValue], of: [AVAssetTrack], at: CMTime) throws

Inserts the time ranges of multiple source tracks into a track of a composition.

func removeTimeRange(CMTimeRange)

Removes a time range of media from a composition track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range of the track.

### Associating Tracks

func addTrackAssociation(to: AVCompositionTrack, type: AVAssetTrack.AssociationType)

Establishes a track association of a specific type between two tracks.

func removeTrackAssociation(to: AVCompositionTrack, type: AVAssetTrack.AssociationType)

Removes an association from a composition track.

### Replacing Format Descriptions

func replaceFormatDescription(CMFormatDescription, with: CMFormatDescription?)

Replaces a format description with another or cancels a previous replacement.

### Validating Segments

func validateSegments([AVCompositionTrackSegment]) throws

Returns a Boolean value that indicates whether a given array of track segments conform to the timing rules for a composition track.

## Relationships

### Inherits From

- AVCompositionTrack

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Mutable compositions

class AVMutableComposition

An object that you use to create a new composition from existing assets.

