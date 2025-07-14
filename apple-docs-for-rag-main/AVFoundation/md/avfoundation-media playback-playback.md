

- AVFoundation
-  Media playback 

API Collection

# Media playback

Manage the playback of media assets and interstitial content, independent of how you present that content in your interface.

## Overview

You use a player to manage the playback and timing of a media asset, for example starting and stopping playback, and seeking to a particular time. A player manages the playback of a single media asset at a time. The framework also provides a queue player that queues media assets to play sequentially.

Note

When you use AVFoundation, Apple may collect metrics to help improve the framework.

You create an instance of AVPlayerItem to play a media asset. A player item manages the timing and presentation state of an asset played by the player. A player item also contains player item tracks that correspond to the tracks in the asset. You direct the output of a player to a specialized Core Animation layer, a player layer, or a synchronized layer.

Important

You must call the VTRegisterProfessionalVideoWorkflowVideoDecoders() function if your app requires Afterburner accelerated playback and decoding of ProRes and ProRes RAW video files.

## Topics

### Essentials

Configuring your app for media playback

Configure apps to enable standard media playback behavior.

### Playback control

Controlling the transport behavior of a player

Play, pause, and seek through a media presentation.

class AVPlayer

An object that provides the interface to control the player’s transport behavior.

class AVPlayerItem

An object that models the timing and presentation state of an asset during playback.

class AVPlayerItemTrack

An object that represents the presentation state of an asset track during playback.

class AVQueuePlayer

An object that plays a sequence of player items.

class AVPlayerLooper

An object that loops media content using a queue player.

### SharePlay

Destination Video

Leverage SwiftUI to build an immersive media experience in a multiplatform app.

Supporting Coordinated Media Playback

Create synchronized media experiences that enable users to watch and listen across devices.

class AVPlaybackCoordinator

An object that coordinates the playback of players in a connected group.

class AVPlayerPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of player objects in a connected group.

class AVDelegatingPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of custom player objects in a connected group.

### Presentation

Monitoring playback progress in your app

Observe the playback of a media asset to update your app’s user-interface state.

Using HEVC Video with Alpha

Play, write, and export HEVC video with an alpha channel to add overlay effects to your video processing.

class AVPlayerLayer

An object that presents the visual contents of a player object.

class AVSynchronizedLayer

A Core Animation layer that derives its timing from a player item so that you can synchronize layer animations with media playback.

### Media selection

Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

### Interstitials

Providing an integrated view of your timeline when playing HLS interstitials

Go beyond simple ad insertion with point and fill occupancy HLS interstitials.

class AVPlayerInterstitialEvent

An object that provides instructions for how a player presents interstitial content.

class AVPlayerInterstitialEventController

An object that schedules interstitial events for items played by the primary player.

class AVPlayerInterstitialEventMonitor

An object that monitors the scheduling and progress of interstitial events.

class AVPlayerItemIntegratedTimeline

An object that models the timeline and playback sequence of a primary player item and scheduled interstitial events.

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricEvent

A base class that represents a metric event.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

### Remote controls

Supporting remote interactions in tvOS

Set up your app to support remote commands and events in a variety of scenarios by using the relevant approach.

### Timed metadata

Presenting Chapter Markers

Add chapter markers to enable users to quickly navigate your content.

class AVMetadataGroup

A collection of metadata items associated with a timeline segment.

class AVTimedMetadataGroup

A collection of metadata items that are valid for use during a specific time range.

class AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

class AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

### Media output

class AVPlayerVideoOutput

An object that receives video data from a player object.

class AVVideoOutputSpecification

An object that specifies the pixel buffer attributes and tag collections handled by a player video output.

class AVPlayerItemOutput

An abstract class that defines the common interface to output media data from a player item.

class AVPlayerItemVideoOutput

An object that outputs video frames from a player item.

class AVPlayerItemLegibleOutput

An object that vends attributed strings for media with a legible characteristic.

class AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

### Utilities

class AVAssetPlaybackAssistant

An object that provides playback information for an asset.

struct AVAssetPlaybackConfigurationOption

A structure that defines playback configuration options for an asset.

## See Also

### Playback

Offline playback and storage

Download streamed content to disk to allow offline playback, and define policies to automatically remove downloaded assets.

Streaming and AirPlay

Stream content wirelessly to other devices using AirPlay, and handle requests involving FairPlay-protected assets.

Sample buffer playback

Create custom controllers to play and synchronize the timing of sample buffer streams.

