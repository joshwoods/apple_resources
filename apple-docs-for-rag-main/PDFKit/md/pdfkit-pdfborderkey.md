

- PDFKit
-  PDFBorderKey 

Structure

# PDFBorderKey

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFBorderKey
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let dashPattern: PDFBorderKey

static let lineWidth: PDFBorderKey

static let style: PDFBorderKey

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

