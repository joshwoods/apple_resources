

- PDFKit
- PDFAnnotation
-  bounds 

Instance Property

# bounds

Returns the bounding box for the annotation in page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
var bounds: NSRect { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var bounds: CGRect { get set }
```

## Return Value

The bounding box for the annotation in page space.

## Discussion

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Managing Annotation Display Characteristics

var alignment: NSTextAlignment

The alignment of the free text and text widget annotation’s text content.

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

var hasAppearanceStream: Bool

Returns a Boolean value that indicates whether the annotation has an appearance stream associated with it.

