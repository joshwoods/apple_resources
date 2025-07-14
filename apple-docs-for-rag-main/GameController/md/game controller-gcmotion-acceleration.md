

- Game Controller
- GCMotion
-  acceleration 

Instance Property

# acceleration

The total acceleration of the controller that includes gravity and the acceleration the user applies to the controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var acceleration: GCAcceleration { get }
```

## See Also

### Accessing Gravity and Acceleration Data

var gravity: GCAcceleration

The gravity acceleration vector from the controller’s reference frame.

var userAcceleration: GCAcceleration

The acceleration that the user applies to the controller.

struct GCAcceleration

A three-dimensional acceleration vector.

