

- AVFoundation
- Media playback
-  Metric event types 

API Collection

# Metric event types

## Topics

### HTTP Live Streaming

class AVMetricMediaResourceRequestEvent

An event that represents a media resource request.

class AVMetricContentKeyRequestEvent

An event that represents a live streaming content key resource request.

class AVMetricHLSMediaSegmentRequestEvent

An event that represents a live streaming media segment resource request.

class AVMetricHLSPlaylistRequestEvent

An event that represents a live streaming playlist resource request.

class AVMetricPlayerItemVariantSwitchStartEvent

An event that represents when the player attempts a variant switch.

class AVMetricPlayerItemVariantSwitchEvent

An event that represents when the player completes a variant switch.

### Buffering

class AVMetricPlayerItemStallEvent

An event that represents when playback stalls.

class AVMetricPlayerItemLikelyToKeepUpEvent

An event that represents when playback is likely to continue without stalling.

class AVMetricPlayerItemInitialLikelyToKeepUpEvent

An event that represents the initial state for whether playback is likely to continue without stalling.

### Transport control

class AVMetricPlayerItemPlaybackSummaryEvent

An event that represents the combined metrics for the entire playback session.

class AVMetricPlayerItemRateChangeEvent

An event that represents when the playback rate changes.

class AVMetricPlayerItemSeekDidCompleteEvent

An event that represents when the playback seek completes.

class AVMetricPlayerItemSeekEvent

An event that represents when a playback seek occurs.

## See Also

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

