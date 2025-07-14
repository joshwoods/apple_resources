

- AppKit
- NSTypesetter
-  lineFragmentPadding 

Instance Property

# lineFragmentPadding

Returns the current line fragment padding, in points.

macOS

``` source
var lineFragmentPadding: CGFloat { get set }
```

## Return Value

The current line fragment padding, in points; that is, the portion on each end of the line fragment rectangle left blank.

## Discussion

Text is inset within the line fragment rectangle by this amount.

## See Also

### Managing text containers

var currentTextContainer: NSTextContainer?

Returns the text container for the text being typeset.

var textContainers: NSArray?

Returns an array containing the text containers belonging to the current layout manager.

