

- AppKit
- NSTextLayoutFragment
-  textLineFragment(for:isUpstreamAffinity:) 

Instance Method

# textLineFragment(for:isUpstreamAffinity:)

Returns a text line fragment from a specific text location in the document.

macOS 14.0+

``` source
func textLineFragment(
    for textLocation: any NSTextLocation,
    isUpstreamAffinity: Bool
) -> NSTextLineFragment?
```

## Parameters 

`textLocation`  

A text location that a text line fragment contains.

`isUpstreamAffinity`  

A Boolean value that indicates whether the text line fragment ends at the text location you provide.

## Return Value

The text line fragment that contains or ends at the text location you provide, or `nil` if there isn’t a match.

## Discussion

Set `isUpstreamAffinity` to true to find a text fragment by its element range end location, such as when you enumerate over line fragments in reverse order. Set `isUpstreamAffinity` to false to find a text fragment that contains `textLocation`.

## See Also

### Getting line fragments

var textLineFragments: [NSTextLineFragment]

An array of text line fragments.

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func textLineFragment(forVerticalOffset: CGFloat, requiresExactMatch: Bool) -> NSTextLineFragment?

Returns the text line fragment for the vertical offset you provide, or the closest text line fragment beyond the vertical offset.

