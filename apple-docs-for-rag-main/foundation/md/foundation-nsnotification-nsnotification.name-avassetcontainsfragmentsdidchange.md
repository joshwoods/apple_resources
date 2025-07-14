

- Foundation
- NSNotification
- NSNotification.Name
-  AVAssetContainsFragmentsDidChange 

Type Property

# AVAssetContainsFragmentsDidChange

A notification the system posts when an asset’s fragments change.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+

``` source
static let AVAssetContainsFragmentsDidChange: NSNotification.Name
```

## Discussion

You can receive notifications of changes to an asset’s fragments after the system loads the value of an asset’s containsFragments property, and you’ve added the asset to an instance of AVFragmentedAssetMinder.

## See Also

### AVFoundation

static let AVAssetChapterMetadataGroupsDidChange: NSNotification.Name

A notification the system posts when an asset’s chapter metadata groups change.

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

class let runtimeErrorNotification: NSNotification.Name

A notification the system posts when an error occurs during a capture session.

