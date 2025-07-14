

- AppKit
- NSPressureConfiguration
-  init(pressureBehavior:) 

Initializer

# init(pressureBehavior:)

Initializes a pressure configuration object with a specified pressure behavior.

macOS 10.10.3+

``` source
init(pressureBehavior: NSEvent.PressureBehavior)
```

## Parameters 

`pressureBehavior`  

An `NSPressureBehavior` value that describes the behavior and progression for responding to pressure events.

## Return Value

A new pressure configuration object of type `NSPressureConfiguration` that describes how pressure events behave and progress.

## Discussion

The initialized pressure configuration object is used to change the behavior and progression of the trackpad when responding to a mouse drag or pressure event sequence.

## See Also

### Related Documentation

enum PressureBehavior

These constants describe the behavior and progression of a pressure gesture.

### Creating a Pressure Configuration Object

func set()

Changes the pressure configuration of the trackpad to the initialized pressure configuration.

