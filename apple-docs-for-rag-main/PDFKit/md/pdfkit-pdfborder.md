

- PDFKit
-  PDFBorder 

Class

# PDFBorder

An optional border for an annotation that lies completely within the annotation rectangle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFBorder
```

## Topics

### Working with Border Styles and Characteristics

var style: PDFBorderStyle

Sets the border style.

enum PDFBorderStyle

PDF Kit annotation borders may have the following styles.

var lineWidth: CGFloat

Sets the line width (in points) for the border.

var dashPattern: [Any]?

Gets the dash pattern for the border as an array of NSNumber objects.

var borderKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of all border properties.

struct PDFBorderKey

### Drawing Borders

func draw(in: CGRect)

Draws the border.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

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

var isHighlighted: Bool

A Boolean value that indicates whether the annotation is in a highlighted state, such as when the mouse is down on a link annotation.

var color: UIColor

Sets the stroke color for the annotation.

var hasAppearanceStream: Bool

Returns a Boolean value that indicates whether the annotation has an appearance stream associated with it.

