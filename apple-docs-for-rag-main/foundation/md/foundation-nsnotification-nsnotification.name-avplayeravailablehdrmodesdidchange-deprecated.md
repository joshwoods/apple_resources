

- Foundation
- NSNotification
- NSNotification.Name
-  AVPlayerAvailableHDRModesDidChange Deprecated

Type Property

# AVPlayerAvailableHDRModesDidChange

A notification the system posts when a player’s available HDR modes change.

iOS 11.2–18.4DeprecatediPadOS 11.2–18.4DeprecatedMac Catalyst 13.1+tvOS 11.2–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
static let AVPlayerAvailableHDRModesDidChange: NSNotification.Name
```

Deprecated

Apple discourages the use of this symbol.

## Discussion

The value of a player’s availableHDRModes may change due to the connection or disconnection of a display, or other change in resources.

## See Also

### AVFoundation

static let AVAssetChapterMetadataGroupsDidChange: NSNotification.Name

A notification the system posts when an asset’s chapter metadata groups change.

static let AVAssetContainsFragmentsDidChange: NSNotification.Name

A notification the system posts when an asset’s fragments change.

static let AVAssetDurationDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset’s duration.

static let AVAssetMediaSelectionGroupsDidChange: NSNotification.Name

A notification the system posts when an asset’s media selection groups change.

static let AVAssetTrackSegmentsDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset track’s segments.

static let AVAssetTrackTimeRangeDidChange: NSNotification.Name

A notification the system posts when a fragmented asset minder observes a change to a fragmented asset track’s time range.

static let AVAssetTrackTrackAssociationsDidChange: NSNotification.Name

A notification the system posts when the track associations for an asset track change.

static let AVAssetWasDefragmented: NSNotification.Name

A notification the system posts when a fragmented asset minder observes that the system defragments the asset on disk.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

class let wasConnectedNotification: NSNotification.Name

A notification the system posts when a new capture device becomes available.

class let wasDisconnectedNotification: NSNotification.Name

A notification the system posts when an existing device becomes unavailable.

class let formatDescriptionDidChangeNotification: NSNotification.Name

A notification the system posts when the capture input port’s format description changes.

class let didStartRunningNotification: NSNotification.Name

A notification the system posts when a capture session starts.

class let didStopRunningNotification: NSNotification.Name

A notification the system posts when a capture session stops.

class let interruptionEndedNotification: NSNotification.Name

A notification the system posts when an interruption to a capture session finishes.

