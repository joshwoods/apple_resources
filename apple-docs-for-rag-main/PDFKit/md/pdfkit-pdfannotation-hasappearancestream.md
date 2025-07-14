

- PDFKit
- PDFAnnotation
-  hasAppearanceStream 

Instance Property

# hasAppearanceStream

Returns a Boolean value that indicates whether the annotation has an appearance stream associated with it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var hasAppearanceStream: Bool { get }
```

## Return Value

true if the annotation has an appearance stream; otherwise false.

## Mentioned in 

Adding Custom Graphics to a PDF

## Discussion

An appearance stream is a sequence of draw instructions used to render a PDF item. If an appearance stream exists, PDF Kit draws the annotation using the stream, which may override existing set parameters (such as the stroke color set with `setColor`).

## See Also

### Managing Annotation Display Characteristics

var alignment: NSTextAlignment

The alignment of the free text and text widget annotation’s text content.

var bounds: CGRect

Returns the bounding box for the annotation in page space.

var contents: String?

Returns the textual content (if any) associated with the annotation.

var font: UIFont?

The font the annotation uses to display text.

var fontColor: UIColor?

The font color the annotation uses to display text.

var border: PDFBorder?

Sets the border style for the annotation.

class PDFBorder

An optional border for an annotation that lies completely within the annotation rectangle.

var isHighlighted: Bool

A Boolean value that indicates whether the annotation is in a highlighted state, such as when the mouse is down on a link annotation.

var color: UIColor

Sets the stroke color for the annotation.

