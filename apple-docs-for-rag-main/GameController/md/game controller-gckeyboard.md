

- Game Controller
-  GCKeyboard 

Class

# GCKeyboard

An object that represents a physical keyboard connected to a device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCKeyboard
```

## Overview

To get the keyboard object and its input values, register for the GCKeyboardDidConnect (Swift) or GCKeyboardDidConnectNotification (Objective-C) notification for when a keyboard connects to the device, or use the coalesced class property. Then get the input values from the keyboard object’s keyboardInput controller profile.

## Topics

### Discovering keyboards

class var coalesced: GCKeyboard?

The keyboard currently connected to the device.

static let GCKeyboardDidConnect: NSNotification.Name

A notification that posts after a keyboard connects to the device.

static let GCKeyboardDidDisconnect: NSNotification.Name

A notification that posts after a single keyboard, or the last of multiple keyboards, disconnects from the device.

### Getting input values

var keyboardInput: GCKeyboardInput?

The controller profile for the keyboard.

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

class GCRacingWheel

An object that represents a physical racing wheel controller connected to a device.

class GCMouse

An object that represents a physical mouse connected to a device.

