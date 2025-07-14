

- Core Animation
- CALayer
-  Action Identifiers 

API Collection

# Action Identifiers

These constants are the predefined action identifiers used by action(forKey:), add(_:forKey:), defaultAction(forKey:), removeAnimation(forKey:), Layer Filters, and the CAAction protocol method run(forKey:object:arguments:).

## Topics

### Constants

let kCAOnOrderIn: String

The identifier that represents the action taken when a layer becomes visible, either as a result being inserted into the visible layer hierarchy or the layer is no longer set as hidden.

let kCAOnOrderOut: String

The identifier that represents the action taken when the layer is removed from the layer hierarchy or is hidden.

let kCATransition: String

The identifier that represents a transition animation.

## See Also

### Constants

struct CAAutoresizingMask

These constants are used by the autoresizingMask property.

struct CAEdgeAntialiasingMask

This mask is used by the edgeAntialiasingMask property.

Identity Transform

Defines the identity transform matrix used by Core Animation.

Scaling Filters

These constants specify the scaling filters used by magnificationFilter and minificationFilter.

struct CATransform3D

The standard transform matrix used throughout Core Animation.

