

- AppKit
- NSLayoutManager
-  limitsLayoutForSuspiciousContents 

Instance Property

# limitsLayoutForSuspiciousContents

A Boolean value that indicates whether the layout manager avoids laying out unusually long or suspicious input.

macOS 10.14+

``` source
var limitsLayoutForSuspiciousContents: Bool { get set }
```

## Discussion

The default value of this property is false, which causes the layout manager to lay out whatever text you give it. Changing the value to true causes the layout manager to generate invalid layout information when it detects potentially suspicious content.

## See Also

### Configuring the global layout manager options

var allowsNonContiguousLayout: Bool

A Boolean value that indicates whether the layout manager allows noncontiguous layout.

var hasNonContiguousLayout: Bool

A Boolean value that indicates whether the layout manager currently has any areas of noncontiguous layout.

var showsInvisibleCharacters: Bool

A Boolean value that indicates whether to substitute visible glyphs for whitespace and other typically invisible characters.

var showsControlCharacters: Bool

A Boolean value that indicates whether the layout manager substitutes visible glyphs for control characters in the layout.

var usesFontLeading: Bool

A Boolean value that indicates whether the layout manager uses the leading of the font.

var backgroundLayoutEnabled: Bool

A Boolean value that indicates whether the layout manager generates glyphs and lays them out when the app’s run loop is idle.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the layout manager uses the default hyphenation rules to wrap lines.

