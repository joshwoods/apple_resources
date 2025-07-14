

- RoomPlan
- RoomCaptureSession
-  stop() 

Instance Method

# stop()

Stops the room-capture session and indicates whether the app pauses the underlying AR session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func stop()
```

## Mentioned in 

Scanning the rooms of a single structure

## See Also

### Controlling a session

func run(configuration: RoomCaptureSession.Configuration)

Start capture process for the session with specified options

struct Configuration

An object to configure the capture process

func stop(pauseARSession: Bool)

