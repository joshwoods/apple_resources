

- RoomPlan
- RoomCaptureSession
-  run(configuration:) 

Instance Method

# run(configuration:)

Start capture process for the session with specified options

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func run(configuration: RoomCaptureSession.Configuration)
```

## Mentioned in 

Scanning the rooms of a single structure

## See Also

### Controlling a session

struct Configuration

An object to configure the capture process

func stop()

Stops the room-capture session and indicates whether the app pauses the underlying AR session.

func stop(pauseARSession: Bool)

