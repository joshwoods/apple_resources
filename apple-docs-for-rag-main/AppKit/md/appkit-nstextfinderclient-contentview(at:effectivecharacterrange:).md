

- AppKit
- NSTextFinderClient
-  contentView(at:effectiveCharacterRange:) 

Instance Method

# contentView(at:effectiveCharacterRange:)

Returns the view the context is displayed in.

macOS

``` source
optional func contentView(
    at index: Int,
    effectiveCharacterRange outRange: NSRangePointer
) -> NSView
```

## Parameters 

`index`  

The index of the view containing the located text.

`outRange`  

Returns, by reference, the entire range of the string displayed by the view

## Return Value

Returns the view the contains the found text.

## See Also

### Determining and Displaying Text Locations

func rects(forCharacterRange: NSRange) -> [NSValue]?

An array containing the located text in the content view’s coordinate system.

func scrollRangeToVisible(NSRange)

Scrolls the specified range such that it is visible.

var visibleCharacterRanges: [NSValue]

An array of visible character ranges.

