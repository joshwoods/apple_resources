

- SwiftUI
- GeometryProxy3D
-  size 

Instance Property

# size

The size of the container view.

visionOS 1.0+

``` source
var size: Size3D { get }
```

## See Also

### Accessing geometry characteristics

func frame(in: some CoordinateSpaceProtocol) -> Rect3D

The container view’s bounds rectangle converted to a defined coordinate space.

var safeAreaInsets: EdgeInsets3D

The safe area inset of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

