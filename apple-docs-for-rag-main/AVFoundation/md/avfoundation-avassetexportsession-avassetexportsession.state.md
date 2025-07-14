

- AVFoundation
- AVAssetExportSession
-  AVAssetExportSession.State 

Enumeration

# AVAssetExportSession.State

Constants that indicate the state of an export operation.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum State
```

## Topics

### States

case pending

An export operation is currently pending.

case exporting(progress: Progress)

An export session is currently exporting media.

case waiting

An export session is currently waiting.

## Relationships

### Conforms To

- Sendable

## See Also

### Monitoring Export Progress

func states(updateInterval: TimeInterval) -> some Sendable &amp; AsyncSequence&lt;AVAssetExportSession.State, Never> 

Monitors the progress state of an export operation.

var status: AVAssetExportSession.Status

The status of the export session.

Deprecated

enum Status

Values that indicate the state of an export session.

var progress: Float

A value that indicates the progress of the export.

Deprecated

var error: (any Error)?

An optional error object.

Deprecated

