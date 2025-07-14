

- AVFoundation
-  Composite assets 

API Collection

# Composite assets

Combine tracks and segments of tracks from multiple assets into a composite asset that you can play or process.

## Topics

### Compositions

class AVComposition

An object that combines and arranges media from multiple assets into a single composite asset that you can play or process.

class AVCompositionTrack

A track in a composition that presents media of a uniform type.

class AVCompositionTrackSegment

A track segment that maps a time from the source media track to the composition track.

### Mutable compositions

class AVMutableComposition

An object that you use to create a new composition from existing assets.

class AVMutableCompositionTrack

A mutable track in a composition that you use to insert, remove, and scale track segments without affecting their low-level representation.

## See Also

### Editing

QuickTime movies

Access the contents of a QuickTime movie file, and perform sample-level edits of its media tracks.

Video effects

Define standard video transition effects, synchronize layer animations with media timing, and create custom video compositors.

Audio mixing

Define how to mix the audio levels from multiple audio tracks over an asset’s duration.

