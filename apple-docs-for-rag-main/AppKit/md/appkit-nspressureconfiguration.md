

- AppKit
-  NSPressureConfiguration 

Class

# NSPressureConfiguration

An encapsulation of the behavior and progression of a Force Touch trackpad as it responds to specific events.

macOS 10.10.3+

``` source
class NSPressureConfiguration
```

## Overview

Use an NSPressureConfiguration object to configure the behavior and progression of a Force Touch trackpad when it responds to a mouse drag or pressure event sequence. Pressure configurations are assigned to views (NSView) and gesture recognizers (NSGestureRecognizer).

## Topics

### Creating a Pressure Configuration Object

init(pressureBehavior: NSEvent.PressureBehavior)

Initializes a pressure configuration object with a specified pressure behavior.

func set()

Changes the pressure configuration of the trackpad to the initialized pressure configuration.

### Accessing Pressure Configuration Object Properties

var pressureBehavior: NSEvent.PressureBehavior

The pressure behavior of the pressure configuration object.

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

### Trackpad

class NSHapticFeedbackManager

An object that provides access to the haptic feedback management attributes on a system with a Force Touch trackpad.

