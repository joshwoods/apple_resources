

- Game Controller
- GCMotion
-  gravity 

Instance Property

# gravity

The gravity acceleration vector from the controller’s reference frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var gravity: GCAcceleration { get }
```

## See Also

### Accessing Gravity and Acceleration Data

var acceleration: GCAcceleration

The total acceleration of the controller that includes gravity and the acceleration the user applies to the controller.

var userAcceleration: GCAcceleration

The acceleration that the user applies to the controller.

struct GCAcceleration

A three-dimensional acceleration vector.

