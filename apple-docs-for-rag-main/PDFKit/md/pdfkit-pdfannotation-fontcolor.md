

- PDFKit
- PDFAnnotation
-  fontColor 

Instance Property

# fontColor

The font color the annotation uses to display text.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@NSCopying
var fontColor: UIColor? { get set }
```

**macOS**

``` source
@NSCopying
var fontColor: NSColor? { get set }
```

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

