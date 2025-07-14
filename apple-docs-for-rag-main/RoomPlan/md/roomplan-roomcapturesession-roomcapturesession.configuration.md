

- RoomPlan
- RoomCaptureSession
-  RoomCaptureSession.Configuration 

Structure

# RoomCaptureSession.Configuration

An object to configure the capture process

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
struct Configuration
```

## Topics

### Creating a configuration

init()

Creates a configuration.

### Configuring a session

var isCoachingEnabled: Bool

An option that indicates that the session periodically provides user instructions.

## See Also

### Controlling a session

func run(configuration: RoomCaptureSession.Configuration)

Start capture process for the session with specified options

func stop()

Stops the room-capture session and indicates whether the app pauses the underlying AR session.

func stop(pauseARSession: Bool)

