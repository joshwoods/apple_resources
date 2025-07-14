

- SwiftUI
- GeometryProxy3D
-  frame(in:) 

Instance Method

# frame(in:)

The container view’s bounds rectangle converted to a defined coordinate space.

visionOS 1.0+

``` source
func frame(in coordinateSpace: some CoordinateSpaceProtocol) -> Rect3D
```

## See Also

### Accessing geometry characteristics

var size: Size3D

The size of the container view.

var safeAreaInsets: EdgeInsets3D

The safe area inset of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

