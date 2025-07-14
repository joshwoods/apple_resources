

- UIKit
- NSMutableParagraphStyle
-  removeTabStop(\_:) 

Instance Method

# removeTabStop(\_:)

Removes the first text tab with a location and type equal to the specified tab stop.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeTabStop(_ anObject: NSTextTab)
```

## See Also

### Related Documentation

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

### Specifying tab information

func addTabStop(NSTextTab)

Adds the specified tab stop to the paragraph.

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

var defaultTabInterval: CGFloat

A number used as the document’s default tab spacing.

