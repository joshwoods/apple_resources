

- PDFKit
- PDFView
-  page(for:nearest:) 

Instance Method

# page(for:nearest:)

Returns the page containing a point specified in view coordinates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func page(
    for point: CGPoint,
    nearest: Bool
) -> PDFPage?
```

**macOS**

``` source
@MainActor
func page(
    for point: NSPoint,
    nearest: Bool
) -> PDFPage?
```

## Discussion

Returns `NULL` if there’s no page at the specified point and `nearest` is set to false.

## See Also

### Converting Page and View Points

func convert(CGPoint, to: PDFPage) -> CGPoint

Converts a point from view space to page space.

func convert(CGRect, to: PDFPage) -> CGRect

Converts a rectangle from view space to page space.

func convert(CGPoint, from: PDFPage) -> CGPoint

Converts a point from page space to view space.

func convert(CGRect, from: PDFPage) -> CGRect

Converts a rectangle from page space to view space.

