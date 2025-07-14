

- Spatial
- Rect3D
-  integral 

Instance Property

# integral

Returns the smallest rectangle after converting the source rectangle values to integers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var integral: Rect3D { get }
```

## See Also

### Creating derived 3D rectangles

func formInset(by: Size3D)

Insets the rectangle by the specified size.

func inset(by: Size3D) -> Rect3D

Returns a new rectangle with the same center point after applying the specified inset amount.

func intersection(Rect3D) -> Rect3D?

Returns the intersection of two rectangles.

var standardized: Rect3D

A rectangle with positive dimensions.

