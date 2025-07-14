

- AVFoundation
-  AVPlayerItemIntegratedTimeline 

Class

# AVPlayerItemIntegratedTimeline

An object that models the timeline and playback sequence of a primary player item and scheduled interstitial events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVPlayerItemIntegratedTimeline
```

## Overview

The timeline models all regions to traverse during playback. A player may not present portions of the primary item when exiting an interstitial event with a positive resumption offset.

## Topics

### Inspecting snapshots

var currentSnapshot: AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of the timeline state at time of request.

class AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of inspectable details of an integrated timeline object.

class let snapshotsOutOfSyncNotification: NSNotification.Name

A notification the system posts when the snapshot objects provided by this timeline become out of sync with the current timeline state.

### Inspecting the time and date

var currentTime: CMTime

The current time on the integrated timeline.

var currentDate: Date?

The current date of playback.

### Seeking

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Seeks to a particular time in the integrated time domain.

func seek(to: Date, completionHandler: ((Bool) -> Void)?)

Seeks to a particular date in the integrated time domain.

### Observing time changes

func periodicTimes(forInterval: CMTime) -> AVPlayerItemIntegratedTimeline.PeriodicTimes

Returns an asynchronous sequence of times periodically as playback progresses.

func boundaryTimes(for: AVPlayerItemSegment, offsetsIntoSegment: [CMTime]) -> AVPlayerItemIntegratedTimeline.BoundaryTimes

Returns an asynchronous sequence of times whenever playback reaches a segment time in the segment.

struct BoundaryTimes

An asynchronous sequence of boundary time values.

struct PeriodicTimes

An asynchronous sequence of periodic time values.

protocol AVPlayerItemIntegratedTimelineObserver

A protocol for objects that perform timeline observations.

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

### Interstitials

Providing an integrated view of your timeline when playing HLS interstitials

Go beyond simple ad insertion with point and fill occupancy HLS interstitials.

class AVPlayerInterstitialEvent

An object that provides instructions for how a player presents interstitial content.

class AVPlayerInterstitialEventController

An object that schedules interstitial events for items played by the primary player.

class AVPlayerInterstitialEventMonitor

An object that monitors the scheduling and progress of interstitial events.

