

- PDFKit
- PDFAnnotation
-  shouldPrint 

Instance Property

# shouldPrint

Returns a Boolean value indicating whether the annotation should appear when the document is printed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var shouldPrint: Bool { get set }
```

## Return Value

true if the annotation should appear when the PDF document is printed; otherwise false.

## Discussion

`PDFPage` respects this flag when printing.

## See Also

### Managing Annotation Drawing and Output

func draw(with: PDFDisplayBox, in: CGContext)

Draws the annotation in a graphics context using page-space coordinates relative to the origin of the specified box.

var shouldDisplay: Bool

Returns a Boolean value indicating whether the annotation should be displayed.

