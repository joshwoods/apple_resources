

- Game Controller
-  GCControllerInputState 

Class

# GCControllerInputState

A class that represents an input state for gamepads and arcade sticks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class GCControllerInputState
```

## Overview

This class implements the GCDevicePhysicalInputState protocol for gamepads and arcade sticks. Instances of this class represent the state of the controller’s inputs at a moment in time, which can be the current time.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GCControllerLiveInput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCDevicePhysicalInputState
- Hashable
- NSObjectProtocol

## See Also

### Accessing controller input

var input: GCControllerLiveInput

The input profile for the controller.

class GCControllerLiveInput

The input profile for a controller.

