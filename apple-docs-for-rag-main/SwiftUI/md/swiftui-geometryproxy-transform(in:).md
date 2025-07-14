

- SwiftUI
- GeometryProxy
-  transform(in:) 

Instance Method

# transform(in:)

The container view’s 3D transform converted to a defined coordinate space.

visionOS 1.0+

``` source
func transform(in coordinateSpace: some CoordinateSpaceProtocol) -> AffineTransform3D?
```

## Discussion

If the view doesn’t have a well defined transform, such as if it is affected by a projection transform, this function may return `nil`.

## See Also

### Accessing geometry characteristics

func bounds(of: NamedCoordinateSpace) -> CGRect?

Returns the given coordinate space’s bounds rectangle, converted to the local coordinate space.

func frame(in:)

Returns the container view’s bounds rectangle, converted to a defined coordinate space.

var size: CGSize

The size of the container view.

var safeAreaInsets: EdgeInsets

The safe area inset of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

