

- SwiftUI
- GeometryProxy3D
-  safeAreaInsets 

Instance Property

# safeAreaInsets

The safe area inset of the container view.

visionOS 1.0+

``` source
var safeAreaInsets: EdgeInsets3D { get }
```

## See Also

### Accessing geometry characteristics

func frame(in: some CoordinateSpaceProtocol) -> Rect3D

The container view’s bounds rectangle converted to a defined coordinate space.

var size: Size3D

The size of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

