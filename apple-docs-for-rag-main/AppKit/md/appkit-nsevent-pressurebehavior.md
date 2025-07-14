

- AppKit
- NSEvent
-  pressureBehavior 

Instance Property

# pressureBehavior

The behavior and progression for a pressure event.

macOS 10.11+

``` source
var pressureBehavior: NSEvent.PressureBehavior { get }
```

## Discussion

This property describes the behavior and progression of an event of type NSEvent.EventType.pressure. The value of this property indicates how the pressure event behaves, including actuations, pressure-level reporting, and stage transitions.

## See Also

### Related Documentation

class NSPressureConfiguration

An encapsulation of the behavior and progression of a Force Touch trackpad as it responds to specific events.

enum EventType

Constants for the types of events that responder objects can handle.

case pressure

An event that reports a change in pressure on a pressure-sensitive device.

init(pressureBehavior: NSEvent.PressureBehavior)

Initializes a pressure configuration object with a specified pressure behavior.

### Getting pressure information

var pressure: Float

A normalized value that indicates the degree of pressure applied to an appropriate input device.

var stage: Int

A value that indicates the stage of a pressure gesture event.

var stageTransition: CGFloat

The transition value for the stage of a pressure gesture event.

enum PressureBehavior

These constants describe the behavior and progression of a pressure gesture.

