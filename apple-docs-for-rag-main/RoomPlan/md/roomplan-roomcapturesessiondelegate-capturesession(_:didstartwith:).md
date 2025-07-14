

- RoomPlan
- RoomCaptureSessionDelegate
-  captureSession(\_:didStartWith:) 

Instance Method

# captureSession(\_:didStartWith:)

Notifies the delegate when the session starts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureSession(
    _ session: RoomCaptureSession,
    didStartWith configuration: RoomCaptureSession.Configuration
)
```

**Required** Default implementation provided.

## Parameters 

`session`  

An object that manages the room-scanning process.

`configuration`  

An object that customizes the scanning experience.

## Default Implementations

### RoomCaptureSessionDelegate Implementations

func captureSession(RoomCaptureSession, didStartWith: RoomCaptureSession.Configuration)

Provides a default, blank implementation for when the session starts.

