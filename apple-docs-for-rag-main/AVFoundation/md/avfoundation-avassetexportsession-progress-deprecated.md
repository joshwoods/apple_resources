

- AVFoundation
- AVAssetExportSession
-  progress Deprecated

Instance Property

# progress

A value that indicates the progress of the export.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7–11.0DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0+

``` source
var progress: Float { get }
```

Deprecated

Use `progressStates(updateInterval:)` instead.

## Discussion

The value of this property ranges from `0.0` to `1.0.`

## See Also

### Monitoring Export Progress

func states(updateInterval: TimeInterval) -> some Sendable &amp; AsyncSequence&lt;AVAssetExportSession.State, Never> 

Monitors the progress state of an export operation.

enum State

Constants that indicate the state of an export operation.

var status: AVAssetExportSession.Status

The status of the export session.

Deprecated

enum Status

Values that indicate the state of an export session.

var error: (any Error)?

An optional error object.

Deprecated

