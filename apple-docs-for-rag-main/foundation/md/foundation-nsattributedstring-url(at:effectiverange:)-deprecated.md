

- Foundation
- NSAttributedString
-  url(at:effectiveRange:) Deprecated

Instance Method

# url(at:effectiveRange:)

Returns a URL, either from a link attribute or from text at the specified location that appears to be a URL string, for use in automatic link detection.

macOS 10.5–10.11Deprecated

``` source
func url(
    at location: Int,
    effectiveRange: NSRangePointer
) -> URL?
```

Deprecated

Use an NSDataDetector object instead.

## Parameters 

`location`  

The character index in the string at which the method checks for a link.

`effectiveRange`  

The actual range covered by the link attribute or URL string, or of non-URL text if no apparent URL is found.

## Return Value

The URL found at `location`.

## See Also

### Deprecated Instance Methods

func draw(with: NSRect, options: NSString.DrawingOptions)

Draws the attributed string with the specified options within the specified rectangle in the current graphics context.

Deprecated

func boundingRect(with: NSSize, options: NSString.DrawingOptions) -> NSRect

Calculates and returns a bounding rectangle for the attributed string using the options specified within the specified rectangle in the current graphics context.

Deprecated

