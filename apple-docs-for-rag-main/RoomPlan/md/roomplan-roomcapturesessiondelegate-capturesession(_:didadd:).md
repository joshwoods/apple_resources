

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didAdd:) 

Instance Method

# captureSession(\_:didAdd:)

Notifies the delegate of newly added surfaces and objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didAdd room: CapturedRoom
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`room`  

A structure that contains the newest surfaces and objects that the framework identifies during the scan.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didAdd: CapturedRoom)

Provides a default, blank implementation for when the capture session adds surfaces and objects to the scan results.

## See Also

### Updating a session

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

session has recently removed surfaces and objects

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

Notifies the delegate when the session changes the dimensions and the transform properties of surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Notifies the delegate when the session updates the scan results.

**Required** Default implementation provided.

