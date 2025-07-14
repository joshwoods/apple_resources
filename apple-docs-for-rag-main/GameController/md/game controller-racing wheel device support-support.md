

- Game Controller
-  Racing wheel device support 

API Collection

# Racing wheel device support

Add support for racing wheel devices in macOS.

## Overview

For macOS apps that support racing wheel devices, follow these steps for your app:

- If you distribute your app through the Mac App Store, add the com.apple.security.device.usb entitlement to your Xcode project.

- To get a racing wheel controller object, register for the GCRacingWheelDidConnect (Swift) or GCRacingWheelDidConnectNotification (Objective-C) and GCRacingWheelDidDisconnect (Swift) or GCRacingWheelDidDisconnectNotification (Objective-C) notifications. Alternatively, check the `GCRacingWheel` connectedRacingWheels class property for the currently connected controllers.

- To start receiving input from a racing wheel controller, invoke the `GCRacingWheel` acquireDevice() method. Then use the relinquishDevice() method when you finish processing input.

- To process the input, set callbacks for the specific racing wheel elements that you want to receive input from. For example, set the valueDidChangeHandler property of the steering wheel and accelerator pedal elements. Get these elements using the wheel and acceleratorPedal properties of the racing wheel’s wheelInput property, as in: `racingWheel.wheelInput.wheel`.

- If you just want the latest value of the steering wheel, use the `GCSteeringWheelElement` absoluteInput property.

- For games that poll for input, set the input buffer size using the inputStateQueueDepth property. In each iteration of your game loop, repeatedly invoke the nextInputState() method until the queue is empty and it returns `nil`.

## Topics

### Racing wheel controller

class GCRacingWheel

An object that represents a physical racing wheel controller connected to a device.

### Racing wheel input

class GCRacingWheelInput

A controller profile that supports a racing wheel.

class GCRacingWheelInputState

The input for the wheel of a racing wheel controller.

### Left and right paddles

var GCInputLeftPaddle: String

The name for the left paddle input.

var GCInputRightPaddle: String

The name for the right paddle input.

### Gear shifter elements

protocol GCAxisInput

The common properties of inputs that provide absolute values along an axis with a fixed origin.

class GCGearShifterElement

An element that represents either a pattern or a sequential gear shift.

protocol GCRelativeInput

The common properties of inputs that provide positions along an axis that are relative to the previous position.

### Steering and switch elements

class GCSteeringWheelElement

The element that represents the wheel of a racing wheel controller.

protocol GCSwitchPositionInput

The common properties of inputs that switch between two or more positions.

### Directional pad elements

protocol GCLinearInput

The common properties of inputs that provide values in unit coordinates.

