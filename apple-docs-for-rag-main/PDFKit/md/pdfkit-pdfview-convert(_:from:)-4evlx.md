

- PDFKit
- PDFView
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a point from page space to view space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ point: CGPoint,
    from page: PDFPage
) -> CGPoint
```

**macOS**

``` source
@MainActor
func convert(
    _ point: NSPoint,
    from page: PDFPage
) -> NSPoint
```

## Discussion

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page. View space is a coordinate system with the origin at the lower-left corner of the current PDF view.

## See Also

### Converting Page and View Points

func page(for: CGPoint, nearest: Bool) -> PDFPage?

Returns the page containing a point specified in view coordinates.

func convert(CGPoint, to: PDFPage) -> CGPoint

Converts a point from view space to page space.

func convert(CGRect, to: PDFPage) -> CGRect

Converts a rectangle from view space to page space.

func convert(CGRect, from: PDFPage) -> CGRect

Converts a rectangle from page space to view space.

