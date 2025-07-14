

- RoomPlan
-  RoomCaptureSession 

Class

# RoomCaptureSession

An object that manages the room-scanning process.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
class RoomCaptureSession
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

This class scans a room on the app’s behalf and provides the necessary callbacks for you to display your own UI.

As an alternate approach to the UX of the framework-provided view (RoomCaptureView), this class is appropriate for apps that intend to display their own view and scanning experience. You can start your own AR experience by accessing this class’s arSession, or by providing your own ARSession instance to the init(arSession:) initializer.

To produce a 3D asset of the user’s environment, this class:

- Utilizes an ARKit session (arSession) that enables the device’s LiDAR Scanner to capture the environment’s physical layout.

- Provides instructions that you display to the user to coach them on moving the device appropriately to collect the necessary data.

## Topics

### Creating a session

init(arSession: ARSession?)

### Ensuring device support

static var isSupported: Bool

A Boolean value that indicates whether the user’s device supports the framework.

### Controlling a session

func run(configuration: RoomCaptureSession.Configuration)

Start capture process for the session with specified options

struct Configuration

An object to configure the capture process

func stop()

Stops the room-capture session and indicates whether the app pauses the underlying AR session.

func stop(pauseARSession: Bool)

### Responding to events

var delegate: (any RoomCaptureSessionDelegate)?

An object that observes important events in the room-scanning process.

enum CaptureError

Errors that can occur during a room-capture session.

### Accessing the AR session

var arSession: ARSession

An object that manages an ARKit session.

### Displaying user instructions

enum Instruction

Capture user instructions

### Initializers

init()

Creates a room-capture session with the given AR session.

## See Also

### Scanning Protocol

protocol RoomCaptureSessionDelegate

A specification of important events in the room-scanning process.

