

- Game Controller
-  GCDeviceHaptics 

Class

# GCDeviceHaptics

The locations of haptic actuators on a game controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCDeviceHaptics
```

## Overview

Use this class to create a haptic engine with a specified locality. Any patterns you send to that engine play on the specified actuators.

Important

The supportsHaptics property of the engine that returns from the createEngine(withLocality:) method applies to the device, not the game controller. Use the supportedLocalities method in this class to determine whether a game controller supports haptics.

## Topics

### Creating a haptics engine

func createEngine(withLocality: GCHapticsLocality) -> CHHapticEngine?

Creates a haptics engine with the specified locality.

let GCHapticDurationInfinite: Float

An infinite duration for a haptics event.

### Getting the localities

var supportedLocalities: Set&lt;GCHapticsLocality>

The locations of haptic actuators on the device.

struct GCHapticsLocality

The location of one or more haptics actuators on a game controller.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Game controller profiles

Input

Receive controller input in the way that best integrates with the flow of your game or game engine.

class GCMotion

A controller profile that supports orientation and motion.

class GCDeviceBattery

The charge level and state of a device’s battery.

class GCDeviceLight

The colored light on a device.

