

- AppKit
- NSMutableParagraphStyle
-  removeTabStop(\_:) 

Instance Method

# removeTabStop(\_:)

Removes the first text tab with a location and type equal to the specified tab stop.

macOS 10.0+

``` source
func removeTabStop(_ anObject: NSTextTab)
```

## See Also

### Specifying tab information

func addTabStop(NSTextTab)

Adds the specified tab stop to the paragraph.

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

var defaultTabInterval: CGFloat

A number used as the document’s default tab spacing.

