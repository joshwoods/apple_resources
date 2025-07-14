

- AppKit
- NSTypesetter
-  currentTextContainer 

Instance Property

# currentTextContainer

Returns the text container for the text being typeset.

macOS

``` source
unowned(unsafe) var currentTextContainer: NSTextContainer? { get }
```

## Return Value

The text container for the text being typeset. This value is valid only while the typesetter is performing layout.

## See Also

### Managing text containers

var textContainers: NSArray?

Returns an array containing the text containers belonging to the current layout manager.

var lineFragmentPadding: CGFloat

Returns the current line fragment padding, in points.

