

- RoomPlan
- RoomBuilder
-  capturedRoom(from:) 

Instance Method

# capturedRoom(from:)

Processes the specified raw scan results and returns a detailed representation of the room.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func capturedRoom(from capturedRoomData: CapturedRoomData) async throws -> CapturedRoom
```

## Parameters 

`capturedRoomData`  

A data object that contains raw scan results.

## Return Value

A captured-room object that provides the key details of a scanned room.

## Discussion

You retrieve the argument `capturedRoomData` in one of the following ways:

- The captureView(shouldPresent:error:) callback for an app that scans rooms using the framework-provided view (RoomCaptureView).

- The captureSession(_:didEndWith:error:) callback for an app that implements its own room-scanning view.

