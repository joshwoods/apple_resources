

- AVFoundation
-  AVPlayerItemIntegratedTimelineSnapshot 

Class

# AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of inspectable details of an integrated timeline object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVPlayerItemIntegratedTimelineSnapshot
```

## Overview

A snapshot doesn’t reflect the new timeline state as playback progresses. You can request a new snapshot instance from an AVPlayerItemIntegratedTimeline that reflect the latest timeline state.

## Topics

### Inspecting the snapshot

var duration: CMTime

The total duration of the primary item and scheduled interstitial events.

var currentSegment: AVPlayerItemSegment?

The currently playing segment.

var segments: [AVPlayerItemSegment]

The segments for this snapshot.

class AVPlayerItemSegment

An immutable object that represents a segment of time on the integrated timeline.

var currentTime: CMTime

The current time on the integrated timeline when the system created the snapshot.

var currentDate: Date?

The current date on the integrated timeline when the system created the snapshot.

### Time mapping

func segmentAndOffsetIntoSegment(forTimelineTime: CMTime) -> (AVPlayerItemSegment, CMTime)

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
- Sendable

## See Also

### Inspecting snapshots

var currentSnapshot: AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of the timeline state at time of request.

class let snapshotsOutOfSyncNotification: NSNotification.Name

A notification the system posts when the snapshot objects provided by this timeline become out of sync with the current timeline state.

