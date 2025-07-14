

- AVFoundation
-  AVPlayerInterstitialEventController 

Class

# AVPlayerInterstitialEventController

An object that schedules interstitial events for items played by the primary player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AVPlayerInterstitialEventController
```

## Overview

This class is a subclass of AVPlayerInterstitialEventMonitor that you use to manage the schedule of interstitial events to present during playback of primary content.

Important

Creating an event controller and setting a schedule causes playback to ignore interstitial events present in the source media.

## Topics

### Creating an Event Controller

init(primaryPlayer: AVPlayer)

Creates an event controller with a player item.

### Configuring the Event Schedule

var events: [AVPlayerInterstitialEvent]!

The current schedule of interstitial events.

func cancelCurrentEvent(withResumptionOffset: CMTime)

Cancels the playback of all currently playing and scheduled interstitial events, and resumes playback of primary content.

## Relationships

### Inherits From

- AVPlayerInterstitialEventMonitor

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

class AVPlayerInterstitialEventMonitor

An object that monitors the scheduling and progress of interstitial events.

class AVPlayerItemIntegratedTimeline

An object that models the timeline and playback sequence of a primary player item and scheduled interstitial events.

