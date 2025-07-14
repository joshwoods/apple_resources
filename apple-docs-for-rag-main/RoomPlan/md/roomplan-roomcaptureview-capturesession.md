

- RoomPlan
- RoomCaptureView
-  captureSession 

Instance Property

# captureSession

An object that notifies a delegate of particular events in the room-scanning life cycle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @preconcurrency
var captureSession: RoomCaptureSession! { get }
```

## Mentioned in 

Scanning the rooms of a single structure

## See Also

### Reacting to scan events

var delegate: (any RoomCaptureViewDelegate)?

An object that determines whether to post-process the results of a scan.

