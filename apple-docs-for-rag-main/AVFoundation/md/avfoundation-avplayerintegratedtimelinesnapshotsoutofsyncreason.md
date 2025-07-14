

- AVFoundation
-  AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason 

Structure

# AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason

Constants that represent the reason for an out-of-sync state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason
```

## Topics

### Getting the reasons

static let segmentsChanged: AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason

The snapshot is out of sync due to a change of segments.

static let currentSegmentChanged: AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason

The snapshot is out of sync due to a change of the current segment.

static let loadedTimeRangesChanged: AVPlayerIntegratedTimelineSnapshotsOutOfSyncReason

The snapshot is out of sync due to a change of the loaded time ranges.

### Creating a reason

init(rawValue: String)

Creates a new out-of-sync reason from the value you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### User-information keys

class let snapshotsOutOfSyncReasonKey: String

A key to retrieve the reason for an out-of-sync state notification.

