

- RoomPlan
- RoomCaptureView
-  delegate 

Instance Property

# delegate

An object that determines whether to post-process the results of a scan.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @preconcurrency
weak var delegate: (any RoomCaptureViewDelegate)?
```

## See Also

### Reacting to scan events

var captureSession: RoomCaptureSession!

An object that notifies a delegate of particular events in the room-scanning life cycle.

