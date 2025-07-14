

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didEndWith:error:) 

Instance Method

# captureSession(\_:didEndWith:error:)

session ends with either CapturedRoom or error

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didEndWith data: CapturedRoomData,
    error: (any Error)?
)
```

## Mentioned in 

Scanning the rooms of a single structure

## See Also

### Default implementations

func captureSession(RoomCaptureSession, didStartWith: RoomCaptureSession.Configuration)

Provides a default, blank implementation for when the session starts.

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Provides a default, blank implementation for when the session updates surfaces and objects during a scan.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

Provides a default, blank implementation for when the session removes surfaces and objects.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

session has changed dimensions and transform properties of surfaces and objects

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

session has user guidance instructions

