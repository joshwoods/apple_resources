

- AppKit
- NSLayoutManager
-  hasNonContiguousLayout 

Instance Property

# hasNonContiguousLayout

A Boolean value that indicates whether the layout manager currently has any areas of noncontiguous layout.

macOS 10.5+

``` source
var hasNonContiguousLayout: Bool { get }
```

## Discussion

There may be times at which there is no noncontiguous layout, such as when layout is complete; this method enables the layout manager to report that to clients.

For more information about noncontiguous layout, see Noncontiguous Layout.

## See Also

### Configuring the global layout manager options

var allowsNonContiguousLayout: Bool

A Boolean value that indicates whether the layout manager allows noncontiguous layout.

var showsInvisibleCharacters: Bool

A Boolean value that indicates whether to substitute visible glyphs for whitespace and other typically invisible characters.

var showsControlCharacters: Bool

A Boolean value that indicates whether the layout manager substitutes visible glyphs for control characters in the layout.

var usesFontLeading: Bool

A Boolean value that indicates whether the layout manager uses the leading of the font.

var backgroundLayoutEnabled: Bool

A Boolean value that indicates whether the layout manager generates glyphs and lays them out when the app’s run loop is idle.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that indicates whether the layout manager avoids laying out unusually long or suspicious input.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the layout manager uses the default hyphenation rules to wrap lines.

