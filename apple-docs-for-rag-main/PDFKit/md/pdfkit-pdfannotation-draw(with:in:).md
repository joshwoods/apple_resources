

- PDFKit
- PDFAnnotation
-  draw(with:in:) 

Instance Method

# draw(with:in:)

Draws the annotation in a graphics context using page-space coordinates relative to the origin of the specified box.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func draw(
    with box: PDFDisplayBox,
    in context: CGContext
)
```

## Parameters 

`box`  

The display box that represents the rectangle to draw the annotation in, in page-space coordinates.

`context`  

The graphics context to draw the annotation in.

## Discussion

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Managing Annotation Drawing and Output

var shouldDisplay: Bool

Returns a Boolean value indicating whether the annotation should be displayed.

var shouldPrint: Bool

Returns a Boolean value indicating whether the annotation should appear when the document is printed.

