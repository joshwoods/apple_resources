

- Game Controller
-  GCRacingWheel 

Class

# GCRacingWheel

An object that represents a physical racing wheel controller connected to a device.

Mac Catalyst 16.0+macOS 13.0+

``` source
class GCRacingWheel
```

## Mentioned in 

Handling input events

## Topics

### Discovering racing wheels

class var connectedRacingWheels: Set&lt;GCRacingWheel>

The racing wheels connected to the device.

static let GCRacingWheelDidConnect: NSNotification.Name

A notification that posts after a racing wheel controller connects to the device.

static let GCRacingWheelDidDisconnect: NSNotification.Name

A notification that posts after a racing wheel controller disconnects from the device.

### Getting events

func acquireDevice() throws

Starts receiving events from the racing wheel.

func relinquishDevice()

Stops receiving events from the racing wheel.

var isAcquired: Bool

A Boolean value that indicates whether the racing wheel sends events to the app.

### Accessing the controller profile

var wheelInput: GCRacingWheelInput

The physical input profile for the racing wheel.

### Creating snapshots

func capture() -> GCRacingWheel

Returns a snapshot of the racing wheel with its current element values.

var isSnapshot: Bool

A Boolean value that indicates whether the object is a snapshot of a racing wheel.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCDevice
- Hashable
- NSObjectProtocol

## See Also

### Game controllers

Supporting Game Controllers

Support a physical controller or add a virtual controller to enhance how people interact with your game through haptics, lighting, and motion sensing.

Letting players use their second-generation Siri Remote as a game controller

Support the second-generation Siri Remote as a game controller in your Apple TV game.

protocol GCDevice

A protocol that defines a common interface for game input devices.

class GCController

A representation of a real game controller, a virtual controller, or a snapshot of a controller.

class GCKeyboard

An object that represents a physical keyboard connected to a device.

class GCMouse

An object that represents a physical mouse connected to a device.

