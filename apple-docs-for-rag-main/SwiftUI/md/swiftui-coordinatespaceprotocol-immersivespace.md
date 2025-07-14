

- SwiftUI
- CoordinateSpaceProtocol
-  immersiveSpace 

Type Property

# immersiveSpace

The named coordinate space that represents the currently opened ImmersiveSpace scene. If no immersive space is currently opened, this CoordinateSpace provides the same behavior as the `.global` coordinate space.

visionOS 1.1+

``` source
static var immersiveSpace: NamedCoordinateSpace { get }
```

Available when `Self` is `NamedCoordinateSpace`.

## See Also

### Getting built-in coordinate spaces

static var global: GlobalCoordinateSpace

The global coordinate space at the root of the view hierarchy.

static var local: LocalCoordinateSpace

The local coordinate space of the current view.

static func named(some Hashable) -> NamedCoordinateSpace

Creates a named coordinate space using the given value.

static var scrollView: NamedCoordinateSpace

The named coordinate space that is added by the system for the innermost containing scroll view.

static func scrollView(axis: Axis) -> Self

The named coordinate space that is added by the system for the innermost containing scroll view that allows scrolling along the provided axis.

