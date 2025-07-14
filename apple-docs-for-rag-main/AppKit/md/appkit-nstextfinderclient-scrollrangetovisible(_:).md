

- AppKit
- NSTextFinderClient
-  scrollRangeToVisible(\_:) 

Instance Method

# scrollRangeToVisible(\_:)

Scrolls the specified range such that it is visible.

macOS

``` source
optional func scrollRangeToVisible(_ range: NSRange)
```

## Parameters 

`range`  

The range to display.

## Discussion

This method is used by all actions, but is not strictly required by any.

## See Also

### Determining and Displaying Text Locations

func contentView(at: Int, effectiveCharacterRange: NSRangePointer) -> NSView

Returns the view the context is displayed in.

func rects(forCharacterRange: NSRange) -> [NSValue]?

An array containing the located text in the content view’s coordinate system.

var visibleCharacterRanges: [NSValue]

An array of visible character ranges.

