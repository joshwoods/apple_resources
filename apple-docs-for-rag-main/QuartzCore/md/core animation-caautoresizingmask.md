

- Core Animation
-  CAAutoresizingMask 

Structure

# CAAutoresizingMask

These constants are used by the autoresizingMask property.

Mac CatalystmacOS

``` source
struct CAAutoresizingMask
```

## Topics

### Constants

init(rawValue: UInt32)

static var layerMinXMargin: CAAutoresizingMask

The left margin between the receiver and its superview is flexible.

static var layerWidthSizable: CAAutoresizingMask

The receiver’s width is flexible.

static var layerMaxXMargin: CAAutoresizingMask

The right margin between the receiver and its superview is flexible.

static var layerMinYMargin: CAAutoresizingMask

The bottom margin between the receiver and its superview is flexible.

static var layerHeightSizable: CAAutoresizingMask

The receiver’s height is flexible.

static var layerMaxYMargin: CAAutoresizingMask

The top margin between the receiver and its superview is flexible.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

Action Identifiers

These constants are the predefined action identifiers used by action(forKey:), add(_:forKey:), defaultAction(forKey:), removeAnimation(forKey:), Layer Filters, and the CAAction protocol method run(forKey:object:arguments:).

struct CAEdgeAntialiasingMask

This mask is used by the edgeAntialiasingMask property.

Identity Transform

Defines the identity transform matrix used by Core Animation.

Scaling Filters

These constants specify the scaling filters used by magnificationFilter and minificationFilter.

struct CATransform3D

The standard transform matrix used throughout Core Animation.

