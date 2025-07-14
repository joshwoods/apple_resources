

- AppKit
- NSLayoutManager
-  usesDefaultHyphenation 

Instance Property

# usesDefaultHyphenation

A Boolean value that indicates whether the layout manager uses the default hyphenation rules to wrap lines.

macOS 10.15+

``` source
var usesDefaultHyphenation: Bool { get set }
```

## Discussion

When the value of this property is true, the layout manager makes a best-effort attempt to hyphenate text when wrapping lines. You may override this hyphenation behavior on a per-paragraph basis using the hyphenationFactor property of NSParagraphStyle The default value of this property is false, which prevents the layout manager from hyphenating text.

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

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that indicates whether the layout manager avoids laying out unusually long or suspicious input.

