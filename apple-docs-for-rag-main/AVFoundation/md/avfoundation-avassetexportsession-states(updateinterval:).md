

- AVFoundation
- AVAssetExportSession
-  states(updateInterval:) 

Instance Method

# states(updateInterval:)

Monitors the progress state of an export operation.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func states(updateInterval: TimeInterval = .infinity) -> some Sendable & AsyncSequence
```

## Parameters 

`updateInterval`  

The time interval between updates. The value must be greater than `0`.

## Return Value

An asynchronous sequence of states.

## See Also

### Monitoring Export Progress

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

var error: (any Error)?

An optional error object.

Deprecated

