

- AppKit
- NSMutableParagraphStyle
-  addTabStop(\_:) 

Instance Method

# addTabStop(\_:)

Adds the specified tab stop to the paragraph.

macOS 10.0+

``` source
func addTabStop(_ anObject: NSTextTab)
```

## See Also

### Specifying tab information

func removeTabStop(NSTextTab)

Removes the first text tab with a location and type equal to the specified tab stop.

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

var defaultTabInterval: CGFloat

A number used as the document’s default tab spacing.

