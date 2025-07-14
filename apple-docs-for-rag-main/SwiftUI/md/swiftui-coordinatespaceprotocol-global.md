

- SwiftUI
- CoordinateSpaceProtocol
-  global 

Type Property

# global

The global coordinate space at the root of the view hierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var global: GlobalCoordinateSpace { get }
```

Available when `Self` is `GlobalCoordinateSpace`.

## See Also

### Getting built-in coordinate spaces

static var immersiveSpace: NamedCoordinateSpace

The named coordinate space that represents the currently opened ImmersiveSpace scene. If no immersive space is currently opened, this CoordinateSpace provides the same behavior as the `.global` coordinate space.

static var local: LocalCoordinateSpace

The local coordinate space of the current view.

static func named(some Hashable) -> NamedCoordinateSpace

Creates a named coordinate space using the given value.

static var scrollView: NamedCoordinateSpace

The named coordinate space that is added by the system for the innermost containing scroll view.

static func scrollView(axis: Axis) -> Self

The named coordinate space that is added by the system for the innermost containing scroll view that allows scrolling along the provided axis.

