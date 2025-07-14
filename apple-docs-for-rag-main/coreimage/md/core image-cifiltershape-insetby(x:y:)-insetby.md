

- Core Image
- CIFilterShape
-  insetBy(x:y:) 

Instance Method

# insetBy(x:y:)

Modifies a filter shape object so that it is inset by the specified x and y values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func insetBy(
    x dx: Int32,
    y dy: Int32
) -> CIFilterShape
```

## Parameters 

`dx`  

A value that specifies an inset in the x direction.

`dy`  

A value that specifies an inset in the y direction.

## See Also

### Modifying a Filter Shape

func intersect(with: CIFilterShape) -> CIFilterShape

Creates a filter shape object that represents the intersection of the current filter shape and the specified filter shape object.

func intersect(with: CGRect) -> CIFilterShape

Creates a filter shape that represents the intersection of the current filter shape and a rectangle.

func transform(by: CGAffineTransform, interior: Bool) -> CIFilterShape

Creates a filter shape that results from applying a transform to the current filter shape.

func union(with: CIFilterShape) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and another filter shape object.

func union(with: CGRect) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and a rectangle.

