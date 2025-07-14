

- Game Controller
- GCController
-  haptics 

Instance Property

# haptics

The controller’s haptics information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var haptics: GCDeviceHaptics? { get }
```

## Discussion

Use this property to create CHHapticEngine instances as necessary in your app. If the controller doesn’t provide haptics information, this property is `nil`.

## See Also

### Accessing battery, haptics, and light objects

var battery: GCDeviceBattery?

The controller’s battery information.

var light: GCDeviceLight?

The controller’s light settings.

