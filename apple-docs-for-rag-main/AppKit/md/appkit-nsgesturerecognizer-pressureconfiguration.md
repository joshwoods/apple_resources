

- AppKit
- NSGestureRecognizer
-  pressureConfiguration 

Instance Property

# pressureConfiguration

Configures the behavior and progression of the Force Touch trackpad when responding to recognized pressure gestures.

macOS 10.11+

``` source
@MainActor
var pressureConfiguration: NSPressureConfiguration { get set }
```

## Discussion

This property contains a value of type NSPressureConfiguration, which configures the behavior and progression of the Force Touch trackpad when responding to recognized pressure gestures.

Ideally, you should avoid changing the pressure configuration during recognition, as the gesture may complete before the configuration has time to take effect. If you do need to change the pressure configuration during recognition, call the set() method of pressureConfiguration.

Once the gesture ends or if recognition fails, the pressure configuration resets to the current view’s pressure configuration, if any, for the remaining duration of the gesture.

## See Also

### Related Documentation

class NSPressureConfiguration

An encapsulation of the behavior and progression of a Force Touch trackpad as it responds to specific events.

enum PressureBehavior

These constants describe the behavior and progression of a pressure gesture.

func set()

Changes the pressure configuration of the trackpad to the initialized pressure configuration.

init(pressureBehavior: NSEvent.PressureBehavior)

Initializes a pressure configuration object with a specified pressure behavior.

