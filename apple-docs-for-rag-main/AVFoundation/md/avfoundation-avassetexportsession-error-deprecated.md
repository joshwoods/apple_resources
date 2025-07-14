

- AVFoundation
- AVAssetExportSession
-  error Deprecated

Instance Property

# error

An optional error object.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var error: (any Error)? { get }
```

Deprecated

Use `export(to:as:)` instead.

## Discussion

The default value of this property is `nil`. The export session sets it to an error object if its status changes to AVAssetExportSession.Status.failed or AVAssetExportSession.Status.cancelled.

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

var progress: Float

A value that indicates the progress of the export.

Deprecated

