

- AppKit
- NSParagraphStyle
-  defaultTabInterval 

Instance Property

# defaultTabInterval

The documentwide default tab interval.

macOS 10.0+

``` source
var defaultTabInterval: CGFloat { get }
```

## Discussion

This property represents the default tab interval in points. Tabs after the last specified in tabStops are placed at integer multiples of this distance (if positive). Default value is 0.0.

## See Also

### Accessing tab information

var tabStops: [NSTextTab]

The text tab objects that represent the paragraph’s tab stops.

enum TextTabType

Constants that specify the type of tab stop.

