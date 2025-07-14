

- AppKit
- NSTextLayoutFragment
-  textLineFragment(forVerticalOffset:requiresExactMatch:) 

Instance Method

# textLineFragment(forVerticalOffset:requiresExactMatch:)

Returns the text line fragment for the vertical offset you provide, or the closest text line fragment beyond the vertical offset.

macOS 14.0+

``` source
func textLineFragment(
    forVerticalOffset verticalOffset: CGFloat,
    requiresExactMatch: Bool
) -> NSTextLineFragment?
```

## Parameters 

`verticalOffset`  

A float value that indicates a vertical distance, expressed in points, from the layout fragment frame’s origin.

`requiresExactMatch`  

A Boolean value that indicates whether the method returns an exact match, or returns the closest match if there isn’t an exact match. The default value is true.

## Return Value

A text line fragment, or `nil` if there isn’t a match.

## Discussion

Set `requiresExactMatch` to true to find the text line fragment that contains the vertical offset, or set `requiresExactMatch` to false to find the closest text line fragment matching or beyond the vertical offset. Returns `nil` if there isn’t a match.

## See Also

### Getting line fragments

var textLineFragments: [NSTextLineFragment]

An array of text line fragments.

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func textLineFragment(for: any NSTextLocation, isUpstreamAffinity: Bool) -> NSTextLineFragment?

Returns a text line fragment from a specific text location in the document.

