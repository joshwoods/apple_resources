

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didStartWith:) 

Instance Method

# captureSession(\_:didStartWith:)

Provides a default, blank implementation for when the session starts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didStartWith configuration: RoomCaptureSession.Configuration
)
```

## Parameters 

`session`  

An object that manages the room-scanning process.

`configuration`  

An object that customizes the scanning experience.

## Discussion

The system calls this implementation if your app doesn’t implement captureSession(_:didStartWith:).

## See Also

### Default implementations

func captureSession(RoomCaptureSession, didUpdate: CapturedRoom)

Provides a default, blank implementation for when the session updates surfaces and objects during a scan.

func captureSession(RoomCaptureSession, didRemove: CapturedRoom)

Provides a default, blank implementation for when the session removes surfaces and objects.

func captureSession(RoomCaptureSession, didChange: CapturedRoom)

session has changed dimensions and transform properties of surfaces and objects

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

session has user guidance instructions

func captureSession(RoomCaptureSession, didEndWith: CapturedRoomData, error: (any Error)?)

session ends with either CapturedRoom or error

