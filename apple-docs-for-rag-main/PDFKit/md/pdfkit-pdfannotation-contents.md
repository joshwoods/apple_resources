

- PDFKit
- PDFAnnotation
-  contents 

Instance Property

# contents

Returns the textual content (if any) associated with the annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var contents: String? { get set }
```

## Return Value

A string representing the textual content associated with the annotation.

## Discussion

Textual content is typically associated with `PDFAnnotationText` and `PDFAnnotationFreeText` annotations.

## See Also

### Related Documentation

var toolTip: String?

Returns text for display as a help tag.

Deprecated

### Managing Annotation Display Characteristics

var alignment: NSTextAlignment

The alignment of the free text and text widget annotation’s text content.

var bounds: CGRect

Returns the bounding box for the annotation in page space.

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

var hasAppearanceStream: Bool

Returns a Boolean value that indicates whether the annotation has an appearance stream associated with it.

