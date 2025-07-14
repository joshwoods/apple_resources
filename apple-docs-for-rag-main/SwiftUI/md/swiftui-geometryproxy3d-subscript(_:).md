

- SwiftUI
- GeometryProxy3D
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Resolves the value of an anchor to the container view.

visionOS 1.0+

``` source
subscript(anchor: Anchor) -> T { get }
```

## See Also

### Accessing geometry characteristics

func frame(in: some CoordinateSpaceProtocol) -> Rect3D

The container view’s bounds rectangle converted to a defined coordinate space.

var size: Size3D

The size of the container view.

var safeAreaInsets: EdgeInsets3D

The safe area inset of the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

