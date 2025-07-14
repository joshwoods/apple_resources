

- AppKit
- NSTypesetter
-  textContainers 

Instance Property

# textContainers

Returns an array containing the text containers belonging to the current layout manager.

macOS

``` source
unowned(unsafe) var textContainers: NSArray? { get }
```

## Return Value

An array containing the text containers belonging to the current layout manager. This value is valid only while the typesetter is performing layout.

## See Also

### Related Documentation

var layoutManager: NSLayoutManager?

Returns the layout manager for the text being typeset.

### Managing text containers

var currentTextContainer: NSTextContainer?

Returns the text container for the text being typeset.

var lineFragmentPadding: CGFloat

Returns the current line fragment padding, in points.

