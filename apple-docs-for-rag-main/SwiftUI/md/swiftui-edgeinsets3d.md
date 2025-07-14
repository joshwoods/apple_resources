

- SwiftUI
-  EdgeInsets3D 

Structure

# EdgeInsets3D

The inset distances for the faces of a 3D volume.

visionOS 1.0+

``` source
@frozen
struct EdgeInsets3D
```

## Topics

### Getting edge insets

var top: CGFloat

The inset distance along the top face of a 3D volume.

var bottom: CGFloat

The inset distance along the bottom face of a 3D volume.

var leading: CGFloat

The inset distance along the leading face of a 3D volume.

var trailing: CGFloat

The inset distance along the top trailing of a 3D volume.

var front: CGFloat

The inset distance along the top front of a 3D volume.

var back: CGFloat

The inset distance along the top back of a 3D volume.

### Creating an edge inset

init(horizontal: CGFloat, vertical: CGFloat, depth: CGFloat)

Creates an `EdgeInsets3D` value with values provided for each axis.

init(top: CGFloat, leading: CGFloat, bottom: CGFloat, trailing: CGFloat, front: CGFloat, back: CGFloat)

Creates an `EdgeInsets3D` value with values provided for each face.

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Accessing edges and regions

enum Edge

An enumeration to indicate one edge of a rectangle.

enum Edge3D

An edge or face of a 3D volume.

enum HorizontalEdge

An edge on the horizontal axis.

enum VerticalEdge

An edge on the vertical axis.

struct EdgeInsets

The inset distances for the sides of a rectangle.

