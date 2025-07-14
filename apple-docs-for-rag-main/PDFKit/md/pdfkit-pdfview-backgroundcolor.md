

- PDFKit
- PDFView
-  backgroundColor 

Instance Property

# backgroundColor

The view’s background color.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@MainActor
var backgroundColor: NSColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var backgroundColor: UIColor { get set }
```

## Discussion

A view’s background is the area displayed to either side of a PDF document’s pages. The background also appears between pages when page breaks are enabled. The default color is a 50% gray.

## See Also

### Setting Background Color

func takeBackgroundColorFrom(Any)

Sets the view’s background color to the specified color.

Deprecated

