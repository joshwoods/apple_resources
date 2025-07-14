

- PDFKit
- PDFBorder
-  style 

Instance Property

# style

Sets the border style.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var style: PDFBorderStyle { get set }
```

## Discussion

Refer to `Constants` for the available border styles.

## See Also

### Working with Border Styles and Characteristics

enum PDFBorderStyle

PDF Kit annotation borders may have the following styles.

var lineWidth: CGFloat

Sets the line width (in points) for the border.

var dashPattern: [Any]?

Gets the dash pattern for the border as an array of NSNumber objects.

var borderKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of all border properties.

struct PDFBorderKey

