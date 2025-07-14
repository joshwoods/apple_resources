

- Spatial
- Rect3D
-  intersection(\_:) 

Instance Method

# intersection(\_:)

Returns the intersection of two rectangles.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func intersection(_ other: Rect3D) -> Rect3D?
```

## Parameters 

`other`  

The rectangle that the function compares against.

## Return Value

A new rectangle that is the intersection of two rectangles.

## See Also

### Creating derived 3D rectangles

var integral: Rect3D

Returns the smallest rectangle after converting the source rectangle values to integers.

func formInset(by: Size3D)

Insets the rectangle by the specified size.

func inset(by: Size3D) -> Rect3D

Returns a new rectangle with the same center point after applying the specified inset amount.

var standardized: Rect3D

A rectangle with positive dimensions.

