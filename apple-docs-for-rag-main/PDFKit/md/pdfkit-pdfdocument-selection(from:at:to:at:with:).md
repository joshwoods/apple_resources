

- PDFKit
- PDFDocument
-  selection(from:at:to:at:with:) 

Instance Method

# selection(from:at:to:at:with:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func selection(
    from startPage: PDFPage,
    at startPoint: CGPoint,
    to endPage: PDFPage,
    at endPoint: CGPoint,
    with granularity: PDFSelectionGranularity
) -> PDFSelection?
```

**macOS**

``` source
func selection(
    from startPage: PDFPage,
    at startPoint: NSPoint,
    to endPage: PDFPage,
    at endPoint: NSPoint,
    with granularity: PDFSelectionGranularity
) -> PDFSelection?
```

