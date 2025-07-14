

- UIKit
- NSTextLayoutFragment
-  textLineFragments 

Instance Property

# textLineFragments

An array of text line fragments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var textLineFragments: [NSTextLineFragment] { get }
```

## Discussion

Valid when NSTextLayoutFragment.State.layoutAvailable. This property is KVO-compliant.

## See Also

### Getting line fragments

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func textLineFragment(for: any NSTextLocation, isUpstreamAffinity: Bool) -> NSTextLineFragment?

Returns a text line fragment from a specific text location in the document.

func textLineFragment(forVerticalOffset: CGFloat, requiresExactMatch: Bool) -> NSTextLineFragment?

Returns the text line fragment for the vertical offset you provide, or the closest text line fragment beyond the vertical offset.

