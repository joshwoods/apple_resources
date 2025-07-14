

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didProvide:) 

Instance Method

# captureSession(\_:didProvide:)

Notifies the delegate of an instruction to display to the user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didProvide instruction: RoomCaptureSession.Instruction
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`instruction`  

A specific recommendation the framework makes for the user to complete the scan.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didProvide: RoomCaptureSession.Instruction)

session has user guidance instructions

