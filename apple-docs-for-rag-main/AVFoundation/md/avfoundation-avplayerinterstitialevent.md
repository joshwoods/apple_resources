

- AVFoundation
-  AVPlayerInterstitialEvent 

Class

# AVPlayerInterstitialEvent

An object that provides instructions for how a player presents interstitial content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AVPlayerInterstitialEvent
```

## Overview

An interstitial event defines a date or time, on the timeline of its primaryItem, at which playback of interstitial content begins. It specifies the alternative interstitial content to play as an array of one or more template player items. The system uses the configuration of the event’s templateItems to build new player item instances to present the interstitial content.

Use AVPlayerInterstitialEventMonitor to observe the scheduling and progress of interstitial events. If your app requires specifying the schedule of interstitial events, use AVPlayerInterstitialEventController instead.

Note

AVPlayerInterstitialEvent was previously an immutable type. Starting in iOS 16, tvOS 16, macOS 13, and watchOS 9, it’s now a mutable type, which allows you to create and customize an event before setting it on an AVPlayerInterstitialEventController.

## Topics

### Creating an event

convenience init(primaryItem: AVPlayerItem, time: CMTime)

Creates an interstitial event for the specified time.

convenience init(primaryItem: AVPlayerItem, date: Date)

Creates an interstitial event for the specified date.

convenience init(primaryItem: AVPlayerItem, identifier: String?, time: CMTime, templateItems: [AVPlayerItem], restrictions: AVPlayerInterstitialEvent.Restrictions, resumptionOffset: CMTime, playoutLimit: CMTime, userDefinedAttributes: [String : Any])

Creates an interstitial event, with user-defined attributes, for the specified time.

convenience init(primaryItem: AVPlayerItem, identifier: String?, date: Date, templateItems: [AVPlayerItem], restrictions: AVPlayerInterstitialEvent.Restrictions, resumptionOffset: CMTime, playoutLimit: CMTime, userDefinedAttributes: [String : Any])

Creates an interstitial event, with user-defined attributes, for the specified date.

### Identifying events

var identifier: String

An identifier for the event.

### Accessing player items

var primaryItem: AVPlayerItem?

The player item that represents the primary content.

var templateItems: [AVPlayerItem]

An array of player item configurations to use as templates for player items that play interstitial content.

### Configuring cues

var cue: AVPlayerInterstitialEvent.Cue

A cue to schedule interstitial event playback at a predefined position during primary playback.

struct Cue

A structure that defines standard cues to play interstitial content.

### Inspecting timing

var time: CMTime

A time within the timeline of the primary content that playback of interstitial content begins.

var date: Date?

A date within the date range of the primary content that playback of interstitial content begins.

var willPlayOnce: Bool

A Boolean value that indicates whether to schedule this event one time only and suppress subsequent replay.

var resumptionOffset: CMTime

A time offset at which playback of primary content resumes after interstitial content finishes.

var playoutLimit: CMTime

The time offset at which playback of the interstitial ends.

var alignsStartWithPrimarySegmentBoundary: Bool

A Boolean value that indicates whether the start time of interstitial playback should snap to a segment boundary of the primary asset.

var alignsResumptionWithPrimarySegmentBoundary: Bool

A Boolean value that indicates whether the resumption time of primary playback should snap to a segment boundary of the primary asset.

### Managing restrictions

var restrictions: AVPlayerInterstitialEvent.Restrictions

The restrictions the event imposes on the playback of interstitial content.

struct Restrictions

Constants that define restrictions on the playback of interstitial content.

### Accessing asset lists

var assetListResponse: [AnyHashable : any Sendable]?

The asset list JSON response as a dictionary.

### Accessing attributes

var userDefinedAttributes: [AnyHashable : any Sendable]

Attributes of the event that the vendor or app defines.

### Inspecting timeline occupancy

var timelineOccupancy: AVPlayerInterstitialEvent.TimelineOccupancy

An event’s occupancy on the integrated timeline.

enum TimelineOccupancy

Constants that specify how an event occupies time on an integrated timeline.

var supplementsPrimaryContent: Bool

A Boolean value that indicates whether an event supplements the primary content and should present with the primary item.

var contentMayVary: Bool

A Boolean value that indicates whether an event’s content is dynamic and the server may respond with different interstitial assets for other participants in a coordinated playback session.

var plannedDuration: CMTime

The planned duration of the event.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Interstitials

Providing an integrated view of your timeline when playing HLS interstitials

Go beyond simple ad insertion with point and fill occupancy HLS interstitials.

class AVPlayerInterstitialEventController

An object that schedules interstitial events for items played by the primary player.

class AVPlayerInterstitialEventMonitor

An object that monitors the scheduling and progress of interstitial events.

class AVPlayerItemIntegratedTimeline

An object that models the timeline and playback sequence of a primary player item and scheduled interstitial events.

