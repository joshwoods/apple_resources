

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didChange:) 

Instance Method

# captureSession(\_:didChange:)

Notifies the delegate when the session changes the dimensions and the transform properties of surfaces and objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didChange room: CapturedRoom
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`room`  

A structure that contains only the surfaces/objects that experience recent changes.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

session has changed dimensions and transform properties of surfaces and objects

## See Also

### Updating a session

func captureSession(RoomCaptureSession, didAdd: CapturedRoom)

Notifies the delegate of newly added surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

session has recently removed surfaces and objects

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Notifies the delegate when the session updates the scan results.

**Required** Default implementation provided.

