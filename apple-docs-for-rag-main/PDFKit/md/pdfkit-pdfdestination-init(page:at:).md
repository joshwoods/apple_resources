

- PDFKit
- PDFDestination
-  init(page:at:) 

Initializer

# init(page:at:)

Initializes the destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
init(
    page: PDFPage,
    at point: NSPoint
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
init(
    page: PDFPage,
    at point: CGPoint
)
```

## Parameters 

`page`  

The page of the destination.

`point`  

The point of the destination, in page space.

## Return Value

An initialized `PDFDestination` instance, or `NULL` if the object could not be initialized.

## Discussion

Specify `point` in page space. Typically, there’s no need to initialize destinations. Instead, you get them from PDFAnnotationLink, PDFOutline, or PDFView objects.

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

