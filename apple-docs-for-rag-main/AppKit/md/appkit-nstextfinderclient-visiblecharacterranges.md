

- AppKit
- NSTextFinderClient
-  visibleCharacterRanges 

Instance Property

# visibleCharacterRanges

An array of visible character ranges.

macOS

``` source
optional var visibleCharacterRanges: [NSValue] { get }
```

## Discussion

The text finder uses this property’s value to determine which ranges it should search to show all of the incremental matches that are currently visible.

If this property is not implemented, then the incremental matches cannot be shown.

The array contains `NSValue` objects that wrap `NSRect` structures.

## See Also

### Determining and Displaying Text Locations

func contentView(at: Int, effectiveCharacterRange: NSRangePointer) -> NSView

Returns the view the context is displayed in.

func rects(forCharacterRange: NSRange) -> [NSValue]?

An array containing the located text in the content view’s coordinate system.

func scrollRangeToVisible(NSRange)

Scrolls the specified range such that it is visible.

