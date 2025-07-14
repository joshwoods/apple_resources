

- SwiftUI
-  EdgeInsets 

Structure

# EdgeInsets

The inset distances for the sides of a rectangle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct EdgeInsets
```

## Topics

### Getting edge insets

var top: CGFloat

var bottom: CGFloat

var leading: CGFloat

var trailing: CGFloat

### Creating an edge inset

init()

init(top: CGFloat, leading: CGFloat, bottom: CGFloat, trailing: CGFloat)

init(_:)

Creates a 2D `EdgeInsets` from an `EdgeInsets3D`, dropping its `front` and `back` values.

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

struct EdgeInsets3D

The inset distances for the faces of a 3D volume.

