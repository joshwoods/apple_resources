

- Foundation
- NSAttributedString
-  boundingRect(with:options:) Deprecated

Instance Method

# boundingRect(with:options:)

Calculates and returns a bounding rectangle for the attributed string using the options specified within the specified rectangle in the current graphics context.

macOS 10.0+

``` source
func boundingRect(
    with size: NSSize,
    options: NSString.DrawingOptions = []
) -> NSRect
```

Deprecated

Use boundingRect(with:options:context:) instead.

## Parameters 

`size`  

The size of the rectangle to draw in.

`options`  

The string drawing options. See NSStringDrawingOptions for the possible values.

## Return Value

The bounding rectangle in the current graphics context.

## Discussion

The origin of the rectangle returned from this method is the first glyph origin.

## See Also

### Deprecated Instance Methods

func url(at: Int, effectiveRange: NSRangePointer) -> URL?

Returns a URL, either from a link attribute or from text at the specified location that appears to be a URL string, for use in automatic link detection.

Deprecated

func draw(with: NSRect, options: NSString.DrawingOptions)

Draws the attributed string with the specified options within the specified rectangle in the current graphics context.

Deprecated

