

- Game Controller
- GCController
-  light 

Instance Property

# light

The controller’s light settings.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var light: GCDeviceLight? { get }
```

## Discussion

Use the light settings to signal the user or to create a more immersive experience. If the controller doesn’t provide light settings, this property is `nil`.

## See Also

### Accessing battery, haptics, and light objects

var battery: GCDeviceBattery?

The controller’s battery information.

var haptics: GCDeviceHaptics?

The controller’s haptics information.

