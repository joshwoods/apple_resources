

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  snapshotsOutOfSyncNotification 

Type Property

# snapshotsOutOfSyncNotification

A notification the system posts when the snapshot objects provided by this timeline become out of sync with the current timeline state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class let snapshotsOutOfSyncNotification: NSNotification.Name
```

## Topics

### User-information keys

class let snapshotsOutOfSyncReasonKey: String

A key to retrieve the reason for an out-of-sync state notification.

struct AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason

Constants that represent the reason for an out-of-sync state.

## See Also

### Inspecting snapshots

var currentSnapshot: AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of the timeline state at time of request.

class AVPlayerItemIntegratedTimelineSnapshot

An immutable representation of inspectable details of an integrated timeline object.

