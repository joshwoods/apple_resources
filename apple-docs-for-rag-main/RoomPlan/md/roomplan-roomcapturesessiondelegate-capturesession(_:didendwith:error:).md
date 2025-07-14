

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didEndWith:error:) 

Instance Method

# captureSession(\_:didEndWith:error:)

Notifies the delegate of completion with either scan results or an error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didEndWith data: CapturedRoomData,
    error: (any Error)?
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`data`  

A data object that contains the raw scan results.

`error`  

An object that describes the problem when an error occurs; otherwise, `nil`.

## Mentioned in 

Scanning the rooms of a single structure

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didEndWith: CapturedRoomData, error: (any Error)?)

session ends with either CapturedRoom or error

