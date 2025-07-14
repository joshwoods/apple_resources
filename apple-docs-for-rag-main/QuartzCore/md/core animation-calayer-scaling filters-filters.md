

- Core Animation
- CALayer
-  Scaling Filters 

API Collection

# Scaling Filters

These constants specify the scaling filters used by magnificationFilter and minificationFilter.

## Topics

### Constants

static let linear: CALayerContentsFilter

Linear interpolation filter.

static let nearest: CALayerContentsFilter

Nearest neighbor interpolation filter.

static let trilinear: CALayerContentsFilter

Trilinear minification filter. Enables mipmap generation. Some renderers may ignore this, or impose additional restrictions, such as source images requiring power-of-two dimensions.

## See Also

### Constants

struct CAAutoresizingMask

These constants are used by the autoresizingMask property.

Action Identifiers

These constants are the predefined action identifiers used by action(forKey:), add(_:forKey:), defaultAction(forKey:), removeAnimation(forKey:), Layer Filters, and the CAAction protocol method run(forKey:object:arguments:).

struct CAEdgeAntialiasingMask

This mask is used by the edgeAntialiasingMask property.

Identity Transform

Defines the identity transform matrix used by Core Animation.

struct CATransform3D

The standard transform matrix used throughout Core Animation.

