

- PDFKit
-  PDFBorderStyle 

Enumeration

# PDFBorderStyle

PDF Kit annotation borders may have the following styles.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
enum PDFBorderStyle
```

## Topics

### Constants

case solid

Solid border.

case dashed

Dashed border.

case beveled

Beveled border.

case inset

Inset border.

case underline

Underline border.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with Border Styles and Characteristics

var style: PDFBorderStyle

Sets the border style.

var lineWidth: CGFloat

Sets the line width (in points) for the border.

var dashPattern: [Any]?

Gets the dash pattern for the border as an array of NSNumber objects.

var borderKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of all border properties.

struct PDFBorderKey

