

- AppKit
- NSText
-  baseWritingDirection 

Instance Property

# baseWritingDirection

The initial writing direction used to determine the actual writing direction for text.

macOS

``` source
@MainActor
var baseWritingDirection: NSWritingDirection { get set }
```

## Discussion

The Text system uses this value as a hint for calculating the actual direction for displaying Unicode characters. If no writing direction is set, returns `NSWritingDirectionNatural`.

