

- Spatial
- Rect3D
-  inset(by:) 

Instance Method

# inset(by:)

Returns a new rectangle with the same center point after applying the specified inset amount.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func inset(by dXYZ: Size3D) -> Rect3D
```

## Parameters 

`dXYZ`  

The size structure that defines the inset values.

## Return Value

A new rectangle with the same center point after applying the specified inset amount.

## See Also

### Creating derived 3D rectangles

var integral: Rect3D

Returns the smallest rectangle after converting the source rectangle values to integers.

func formInset(by: Size3D)

Insets the rectangle by the specified size.

func intersection(Rect3D) -> Rect3D?

Returns the intersection of two rectangles.

var standardized: Rect3D

A rectangle with positive dimensions.

