

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didUpdate:) 

Instance Method

# captureSession(\_:didUpdate:)

Notifies the delegate when the session updates the scan results.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didUpdate room: CapturedRoom
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`room`  

A structure that represents a snapshot of the room being captured.

## Discussion

The `room` structure contains all surfaces/objects in the captured room regardless of the recent changes.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Provides a default, blank implementation for when the session updates surfaces and objects during a scan.

## See Also

### Updating a session

func captureSession(RoomCaptureSession, didAdd: CapturedRoom)

Notifies the delegate of newly added surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

session has recently removed surfaces and objects

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

Notifies the delegate when the session changes the dimensions and the transform properties of surfaces and objects.

**Required** Default implementation provided.

