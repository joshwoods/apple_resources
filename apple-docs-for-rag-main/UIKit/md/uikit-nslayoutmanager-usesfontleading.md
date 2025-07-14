

- UIKit
- NSLayoutManager
-  usesFontLeading 

Instance Property

# usesFontLeading

A Boolean value that indicates whether the layout manager uses the leading of the font.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var usesFontLeading: Bool { get set }
```

## See Also

### Related Documentation

var lineSpacing: CGFloat

The distance in points between the bottom of one line fragment and the top of the next.

### Configuring the global layout manager options

var allowsNonContiguousLayout: Bool

A Boolean value that indicates whether the layout manager allows noncontiguous layout.

var hasNonContiguousLayout: Bool

A Boolean value that indicates whether the layout manager currently has any areas of noncontiguous layout.

var showsInvisibleCharacters: Bool

A Boolean value that indicates whether to substitute visible glyphs for whitespace and other typically invisible characters.

var showsControlCharacters: Bool

A Boolean value that indicates whether the layout manager substitutes visible glyphs for control characters in the layout.

var backgroundLayoutEnabled: Bool { get set }

A Boolean value that indicates whether the layout manager generates glyphs and lays them out when the app’s run loop is idle.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that indicates whether the layout manager avoids laying out unusually long or suspicious input.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the layout manager uses the default hyphenation rules to wrap lines.

