

- SwiftUI
- GeometryProxy
-  frame(in:) 

Instance Method

# frame(in:)

Returns the container view’s bounds rectangle, converted to a defined coordinate space.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func frame(in coordinateSpace: some CoordinateSpaceProtocol) -> CGRect
```

Show all declarations

## See Also

### Accessing geometry characteristics

func bounds(of: NamedCoordinateSpace) -> CGRect?

Returns the given coordinate space’s bounds rectangle, converted to the local coordinate space.

var size: CGSize

The size of the container view.

var safeAreaInsets: EdgeInsets

The safe area inset of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

