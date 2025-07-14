

- PDFKit
- PDFView
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a rectangle from view space to page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@MainActor
func convert(
    _ rect: NSRect,
    to page: PDFPage
) -> NSRect
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ rect: CGRect,
    to page: PDFPage
) -> CGRect
```

## Discussion

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page. View space is a coordinate system with the origin at the lower-left corner of the current PDF view.

## See Also

### Converting Page and View Points

func page(for: CGPoint, nearest: Bool) -> PDFPage?

Returns the page containing a point specified in view coordinates.

func convert(CGPoint, to: PDFPage) -> CGPoint

Converts a point from view space to page space.

func convert(CGPoint, from: PDFPage) -> CGPoint

Converts a point from page space to view space.

func convert(CGRect, from: PDFPage) -> CGRect

Converts a rectangle from page space to view space.

