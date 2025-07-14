

- PDFKit
- PDFBorder
-  lineWidth 

Instance Property

# lineWidth

Sets the line width (in points) for the border.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var lineWidth: CGFloat { get set }
```

## See Also

### Working with Border Styles and Characteristics

var style: PDFBorderStyle

Sets the border style.

enum PDFBorderStyle

PDF Kit annotation borders may have the following styles.

var dashPattern: [Any]?

Gets the dash pattern for the border as an array of NSNumber objects.

var borderKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of all border properties.

struct PDFBorderKey

