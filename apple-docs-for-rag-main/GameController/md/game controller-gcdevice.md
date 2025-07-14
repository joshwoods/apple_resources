

- Game Controller
-  GCDevice 

Protocol

# GCDevice

A protocol that defines a common interface for game input devices.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol GCDevice : NSObjectProtocol
```

## Overview

This protocol provides common properties for game controllers, and mouse and keyboard devices.

## Topics

### Getting device information

var vendorName: String?

The manufacturer-provided name for the device, or the user’s name for the device.

**Required**

var productCategory: String

The product category that identifies the type of controller.

**Required**

Product category constants

### Handling input

var handlerQueue: dispatch_queue_t

The dispatch queue that the framework uses to call element value change handlers.

**Required**

var physicalInputProfile: GCPhysicalInputProfile

The device’s physical input profile, such as a controller’s extended gamepad.

**Required**

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- GCController
- GCKeyboard
- GCMouse
- GCRacingWheel

## See Also

### Game controllers

Supporting Game Controllers

Support a physical controller or add a virtual controller to enhance how people interact with your game through haptics, lighting, and motion sensing.

Letting players use their second-generation Siri Remote as a game controller

Support the second-generation Siri Remote as a game controller in your Apple TV game.

class GCController

A representation of a real game controller, a virtual controller, or a snapshot of a controller.

class GCRacingWheel

An object that represents a physical racing wheel controller connected to a device.

class GCKeyboard

An object that represents a physical keyboard connected to a device.

class GCMouse

An object that represents a physical mouse connected to a device.

