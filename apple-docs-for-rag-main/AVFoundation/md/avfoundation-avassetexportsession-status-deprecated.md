

- AVFoundation
- AVAssetExportSession
-  status Deprecated

Instance Property

# status

The status of the export session.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var status: AVAssetExportSession.Status { get }
```

Deprecated

Use `progressStates(updateInterval:)` instead.

## Discussion

For possible values, see AVAssetExportSession.Status.

This value is key-value observable.

## See Also

### Monitoring Export Progress

func states(updateInterval: TimeInterval) -> some Sendable &amp; AsyncSequence&lt;AVAssetExportSession.State, Never> 

Monitors the progress state of an export operation.

enum State

Constants that indicate the state of an export operation.

enum Status

Values that indicate the state of an export session.

var progress: Float

A value that indicates the progress of the export.

Deprecated

var error: (any Error)?

An optional error object.

Deprecated

