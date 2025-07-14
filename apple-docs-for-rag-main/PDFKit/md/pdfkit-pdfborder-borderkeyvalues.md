

- PDFKit
- PDFBorder
-  borderKeyValues 

Instance Property

# borderKeyValues

A dictionary that contains a deep copy of all border properties.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var borderKeyValues: [AnyHashable : Any] { get }
```

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

struct PDFBorderKey

