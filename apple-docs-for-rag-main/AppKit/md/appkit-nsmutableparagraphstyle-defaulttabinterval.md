

- AppKit
- NSMutableParagraphStyle
-  defaultTabInterval 

Instance Property

# defaultTabInterval

A number used as the document’s default tab spacing.

macOS 10.0+

``` source
var defaultTabInterval: CGFloat { get set }
```

## Discussion

This property represents the default tab interval in points. The system places tabs after the last specified in tabStops at integer multiples of this distance (if positive). Default value is `0.0`.

## See Also

### Specifying tab information

func addTabStop(NSTextTab)

Adds the specified tab stop to the paragraph.

func removeTabStop(NSTextTab)

Removes the first text tab with a location and type equal to the specified tab stop.

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

