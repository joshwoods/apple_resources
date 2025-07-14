

- PDFKit
- PDFAnnotationMarkup
-  setQuadrilateralPoints(\_:) Deprecated

Instance Method

# setQuadrilateralPoints(\_:)

Sets the array of quadrilateral points defining the bounds of the markup.

macOS 10.4–10.12Deprecated

``` source
func setQuadrilateralPoints(_ points: [Any]!)
```

## Discussion

The points defined by each quadrilateral array should encompass a word or a contiguous group of words. The quadrilateral points are ordered counterclockwise, with the first point closest to the origin in page space.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Working with Markup Boundaries

func quadrilateralPoints() -> [Any]!

Gets the array of quadrilateral points defining the bounds of the markup.

Deprecated

