

- Spatial
- Rect3D
-  formInset(by:) 

Instance Method

# formInset(by:)

Insets the rectangle by the specified size.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func formInset(by dXYZ: Size3D)
```

## Parameters 

`dXYZ`  

The size structure that defines the inset values.

## See Also

### Creating derived 3D rectangles

var integral: Rect3D

Returns the smallest rectangle after converting the source rectangle values to integers.

func inset(by: Size3D) -> Rect3D

Returns a new rectangle with the same center point after applying the specified inset amount.

func intersection(Rect3D) -> Rect3D?

Returns the intersection of two rectangles.

var standardized: Rect3D

A rectangle with positive dimensions.

