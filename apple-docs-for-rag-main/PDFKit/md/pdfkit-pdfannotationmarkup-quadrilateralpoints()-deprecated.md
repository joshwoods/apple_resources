

- PDFKit
- PDFAnnotationMarkup
-  quadrilateralPoints() Deprecated

Instance Method

# quadrilateralPoints()

Gets the array of quadrilateral points defining the bounds of the markup.

macOS 10.4–10.12Deprecated

``` source
func quadrilateralPoints() -> [Any]!
```

## Discussion

Each quadrilateral encompasses a word or a contiguous group of words. The quadrilateral points are ordered counterclockwise, with the first point closest to the origin in page space.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Working with Markup Boundaries

func setQuadrilateralPoints([Any]!)

Sets the array of quadrilateral points defining the bounds of the markup.

Deprecated

