

- Game Controller
-  GCDeviceBattery 

Class

# GCDeviceBattery

The charge level and state of a device’s battery.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GCDeviceBattery
```

## Overview

Use this class to display the state of a device’s battery to a player.

## Topics

### Getting the battery level and state

var batteryLevel: Float

The charge level of a device’s battery.

var batteryState: GCDeviceBattery.State

The state of a device’s battery.

enum State

A state that indicates whether a device’s battery has power and is charging.

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

class GCDeviceHaptics

The locations of haptic actuators on a game controller.

class GCDeviceLight

The colored light on a device.

