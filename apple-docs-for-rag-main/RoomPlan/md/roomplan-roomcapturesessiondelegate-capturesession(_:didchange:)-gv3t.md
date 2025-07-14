

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didChange:) 

Instance Method

# captureSession(\_:didChange:)

session has changed dimensions and transform properties of surfaces and objects

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didChange room: CapturedRoom
)
```

## See Also

### Default implementations

func captureSession(RoomCaptureSession, didStartWith: RoomCaptureSession.Configuration)

Provides a default, blank implementation for when the session starts.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Provides a default, blank implementation for when the session updates surfaces and objects during a scan.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

Provides a default, blank implementation for when the session removes surfaces and objects.

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

session has user guidance instructions

func captureSession(RoomCaptureSession, didEndWith: CapturedRoomData, error: (any Error)?)

session ends with either CapturedRoom or error

