

- Core Image
- CIFilterShape
-  intersect(with:) 

Instance Method

# intersect(with:)

Creates a filter shape object that represents the intersection of the current filter shape and the specified filter shape object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func intersect(with s2: CIFilterShape) -> CIFilterShape
```

## Parameters 

`s2`  

A filter shape object.

## Return Value

The filter shape object that results from the intersection.

## See Also

### Modifying a Filter Shape

func insetBy(x: Int32, y: Int32) -> CIFilterShape

Modifies a filter shape object so that it is inset by the specified x and y values.

func intersect(with: CGRect) -> CIFilterShape

Creates a filter shape that represents the intersection of the current filter shape and a rectangle.

func transform(by: CGAffineTransform, interior: Bool) -> CIFilterShape

Creates a filter shape that results from applying a transform to the current filter shape.

func union(with: CIFilterShape) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and another filter shape object.

func union(with: CGRect) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and a rectangle.

