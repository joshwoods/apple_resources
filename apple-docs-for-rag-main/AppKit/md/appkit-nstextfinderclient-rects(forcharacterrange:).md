

- AppKit
- NSTextFinderClient
-  rects(forCharacterRange:) 

Instance Method

# rects(forCharacterRange:)

An array containing the located text in the content view’s coordinate system.

macOS

``` source
optional func rects(forCharacterRange range: NSRange) -> [NSValue]?
```

## Parameters 

`range`  

The range of the located character string.

## Return Value

An array containing the rectangles containing the located text in the content view object’s coordinate system and return that array. The rectangles are return wrapped as `NSValue` objects.

## Discussion

The text finder uses this method to determine the location to display the find indicator.

The given range is guaranteed not to overlap multiple views.

## See Also

### Determining and Displaying Text Locations

func contentView(at: Int, effectiveCharacterRange: NSRangePointer) -> NSView

Returns the view the context is displayed in.

func scrollRangeToVisible(NSRange)

Scrolls the specified range such that it is visible.

var visibleCharacterRanges: [NSValue]

An array of visible character ranges.

