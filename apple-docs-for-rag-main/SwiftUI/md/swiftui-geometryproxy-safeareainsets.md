

- SwiftUI
- GeometryProxy
-  safeAreaInsets 

Instance Property

# safeAreaInsets

The safe area inset of the container view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var safeAreaInsets: EdgeInsets { get }
```

## See Also

### Accessing geometry characteristics

func bounds(of: NamedCoordinateSpace) -> CGRect?

Returns the given coordinate space’s bounds rectangle, converted to the local coordinate space.

func frame(in:)

Returns the container view’s bounds rectangle, converted to a defined coordinate space.

var size: CGSize

The size of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

