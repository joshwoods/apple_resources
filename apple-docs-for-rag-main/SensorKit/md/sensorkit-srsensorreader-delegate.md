

- SensorKit
- SRSensorReader
-  delegate 

Instance Property

# delegate

An object that responds to sensor-related events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
weak var delegate: (any SRSensorReaderDelegate)? { get set }
```

## See Also

### Responding to sensor events

protocol SRSensorReaderDelegate

A set of callbacks the framework invokes to notify the app of sensor-related events.

