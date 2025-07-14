

- Nearby Interaction
- NINearbyAccessoryConfiguration
-  isCameraAssistanceEnabled 

Instance Property

# isCameraAssistanceEnabled

A Boolean value that combines the spatial awareness of ARKit with Nearby Interaction to improve the accuracy of a nearby object’s position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var isCameraAssistanceEnabled: Bool { get set }
```

## Discussion

The default value is `false`.

When `true`, this property leverages ARKit to provide a nearby object’s distance and direction in a wider range of environmental conditions.

By studying image captures from the device’s camera, ARKit creates an accurate world model of the user’s physical space. As the user moves, ARKit tracks the device with 6 degrees of freedom, by noting the device’s:

- 3D position `(x, y, z)`

- 3D orientation `(roll, pitch, yaw)`

Nearby Interaction adds readings from the device’s Ultra Wideband chip to attain a robust position for a nearby object. This also enables the interaction session to provide an object’s horizontalAngle and verticalDirectionEstimate.

