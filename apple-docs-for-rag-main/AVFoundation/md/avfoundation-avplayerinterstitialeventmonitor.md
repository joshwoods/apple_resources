

- AVFoundation
-  AVPlayerInterstitialEventMonitor 

Class

# AVPlayerInterstitialEventMonitor

An object that monitors the scheduling and progress of interstitial events.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AVPlayerInterstitialEventMonitor
```

## Overview

This object monitors interstitial events that exist within the content of the primary items, such as events defined by an HLS media playlist, and also events managed by an AVPlayerInterstitialEventController object. You can access the schedule of interstitial events through the events property.

When it’s time to present an interstitial event, the system suspends playback of the primary item and changes its player’s timeControlStatus to AVPlayer.TimeControlStatus.waitingToPlayAtSpecifiedRate with a reasonForWaitingToPlay value of interstitialEvent. When the system suspends primary playback, it creates player items based on the event’s templateItems to play interstitial content. The interstitial player temporarily assumes the primary player’s output configuration, such as routing its visual output to player layers that reference the primary player. After the interstitial player finishes playback, or its current item otherwise becomes `nil`, playback of primary content resumes.

## Topics

### Creating a monitor

init(primaryPlayer: AVPlayer)

Creates an observer with a player item.

### Monitoring the current event

var currentEvent: AVPlayerInterstitialEvent?

The current interstitial event.

class let currentEventDidChangeNotification: NSNotification.Name

A notification the system posts when the monitor’s current interstitial event changes.

### Monitoring the event schedule

var events: [AVPlayerInterstitialEvent]

The schedule of interstitial events.

class let eventsDidChangeNotification: NSNotification.Name

A notification the system posts when the monitor’s schedule of interstitial events changes.

### Monitoring the asset list response

class let assetListResponseStatusDidChangeNotification: NSNotification.Name

A notification the system posts when the status of an interstitial event’s asset list response changes.

enum AVPlayerInterstitialEventAssetListResponseStatus

Constants that describe the status of the asset list response for an interstitial event.

### Accessing the players

var primaryPlayer: AVPlayer?

An object that plays primary content.

var interstitialPlayer: AVQueuePlayer

An object that plays interstitial content.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVPlayerInterstitialEventController

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

class AVPlayerItemIntegratedTimeline

An object that models the timeline and playback sequence of a primary player item and scheduled interstitial events.

