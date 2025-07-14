

- Game Controller
- GCController
-  battery 

Instance Property

# battery

The controller’s battery information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying
var battery: GCDeviceBattery? { get }
```

## Discussion

Use this property to display the battery life or to warn the user when the controller’s battery level is low. If the controller doesn’t provide battery information, this property is `nil`.

## See Also

### Accessing battery, haptics, and light objects

var haptics: GCDeviceHaptics?

The controller’s haptics information.

var light: GCDeviceLight?

The controller’s light settings.

