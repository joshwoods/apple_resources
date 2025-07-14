

- AVFoundation
- AVAssetExportSession
-  AVAssetExportSession.Status 

Enumeration

# AVAssetExportSession.Status

Values that indicate the state of an export session.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum Status
```

## Topics

### Status Values

case unknown

The session status is unknown.

case waiting

The session is waiting to export more data.

case exporting

The export is in progress.

case completed

The export completes successfully.

case failed

The export fails.

case cancelled

You canceled the export.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Monitoring Export Progress

func states(updateInterval: TimeInterval) -> some Sendable &amp; AsyncSequence&lt;AVAssetExportSession.State, Never> 

Monitors the progress state of an export operation.

enum State

Constants that indicate the state of an export operation.

var status: AVAssetExportSession.Status

The status of the export session.

Deprecated

var progress: Float

A value that indicates the progress of the export.

Deprecated

var error: (any Error)?

An optional error object.

Deprecated

