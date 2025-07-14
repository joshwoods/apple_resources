

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didRemove:) 

Instance Method

# captureSession(\_:didRemove:)

session has recently removed surfaces and objects

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didRemove room: CapturedRoom
)
```

**Required** Default implementation provided.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

Provides a default, blank implementation for when the session removes surfaces and objects.

## See Also

### Updating a session

func captureSession(RoomCaptureSession, didAdd: CapturedRoom)

Notifies the delegate of newly added surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

Notifies the delegate when the session changes the dimensions and the transform properties of surfaces and objects.

**Required** Default implementation provided.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Notifies the delegate when the session updates the scan results.

**Required** Default implementation provided.

