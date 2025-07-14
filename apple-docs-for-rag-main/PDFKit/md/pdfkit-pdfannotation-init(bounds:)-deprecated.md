

- PDFKit
- PDFAnnotation
-  init(bounds:) Deprecated

Initializer

# init(bounds:)

Creates a PDF annotation object.

macOS 10.4–10.12Deprecated

``` source
convenience init(bounds: NSRect)
```

Deprecated

Use init(bounds:forType:withProperties:) instead.

## Parameters 

`bounds`  

The bounding box of the annotation in page-space coordinates.

## Return Value

An initialized `PDFAnnotation` instance, or `NULL` if the object can’t initialize.

## Discussion

Subclasses of `PDFAnnotation` use this method to initialize annotation instances. Provide `bounds` in page-space coordinates. Invoking `initWithBounds:` directly on a `PDFAnnotation` object creates an illegal `NULL` type.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Deprecated Methods

convenience init(dictionary: [AnyHashable : Any], forPage: PDFPage?)Deprecated

func removeAllAppearanceStreams()Deprecated

func draw(with: PDFDisplayBox)

Draws the annotation on its associated page.

Deprecated

