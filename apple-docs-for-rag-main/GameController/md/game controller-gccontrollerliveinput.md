

- Game Controller
-  GCControllerLiveInput 

Class

# GCControllerLiveInput

The input profile for a controller.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class GCControllerLiveInput
```

## Mentioned in 

Handling input events

## Overview

Instances of GCControllerLiveInput represent the current input state of a controller. You can save snapshots of the input state and receive callbacks when the input state changes. You can also get the elements of the controller and their current input values from GCControllerLiveInput instances.

Use the capture() method to save a copy of the current input state. If you want Game Controller to buffer snapshots of the input states for you, use the  inputStateQueueDepth property to set the buffer’s queue depth to a value other than `0`. Then use the nextInputState() method to get the snapshots when you’re ready to process input.

## Topics

### Handling device input

func nextInputState() -> (any GCControllerInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next device input state from the queue.

func capture() -> GCControllerInputState

Returns a snapshot of the physical device inputs.

### Remapping controls

var unmapped: GCControllerLiveInput?

The live input of a controller without any system-level remapping of the controls.

## Relationships

### Inherits From

- GCControllerInputState

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCDevicePhysicalInput
- GCDevicePhysicalInputState
- Hashable
- NSObjectProtocol

## See Also

### Accessing controller input

var input: GCControllerLiveInput

The input profile for the controller.

class GCControllerInputState

A class that represents an input state for gamepads and arcade sticks.

