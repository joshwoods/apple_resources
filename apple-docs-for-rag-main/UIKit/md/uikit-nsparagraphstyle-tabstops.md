

- UIKit
- NSParagraphStyle
-  tabStops 

Instance Property

# tabStops

The text tab objects that represent the paragraph’s tab stops.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var tabStops: [NSTextTab] { get }
```

## Discussion

The NSTextTab objects, sorted by location, define the tab stops for the paragraph style. The default value is an array of 12 left-aligned tabs at 28-point intervals.

## See Also

### Accessing tab information

enum TextTabType

Constants that specify the type of tab stop.

var defaultTabInterval: CGFloat

The documentwide default tab interval.

