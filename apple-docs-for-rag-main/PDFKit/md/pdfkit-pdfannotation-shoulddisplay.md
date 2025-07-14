

- PDFKit
- PDFAnnotation
-  shouldDisplay 

Instance Property

# shouldDisplay

Returns a Boolean value indicating whether the annotation should be displayed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var shouldDisplay: Bool { get set }
```

## Return Value

true if the annotation should be displayed; otherwise false.

## Discussion

`PDFPage` respects this flag when drawing.

## See Also

### Managing Annotation Drawing and Output

func draw(with: PDFDisplayBox, in: CGContext)

Draws the annotation in a graphics context using page-space coordinates relative to the origin of the specified box.

var shouldPrint: Bool

Returns a Boolean value indicating whether the annotation should appear when the document is printed.

