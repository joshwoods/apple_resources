

- Core Image
- CIFilterShape
-  transform(by:interior:) 

Instance Method

# transform(by:interior:)

Creates a filter shape that results from applying a transform to the current filter shape.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func transform(
    by m: CGAffineTransform,
    interior flag: Bool
) -> CIFilterShape
```

## Parameters 

`m`  

A transform.

`flag`  

`false` specifies that the new filter shape object can contain all the pixels in the transformed shape (and possibly some that are outside the transformed shape). `true` specifies that the new filter shape object can contain a subset of the pixels in the transformed shape (but none of those outside the transformed shape).

## Return Value

The transformed filter shape object.

## See Also

### Modifying a Filter Shape

func insetBy(x: Int32, y: Int32) -> CIFilterShape

Modifies a filter shape object so that it is inset by the specified x and y values.

func intersect(with: CIFilterShape) -> CIFilterShape

Creates a filter shape object that represents the intersection of the current filter shape and the specified filter shape object.

func intersect(with: CGRect) -> CIFilterShape

Creates a filter shape that represents the intersection of the current filter shape and a rectangle.

func union(with: CIFilterShape) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and another filter shape object.

func union(with: CGRect) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and a rectangle.

