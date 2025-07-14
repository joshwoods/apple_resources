

- UIKit
- NSLayoutManager
-  hyphenationFactor Deprecated

Instance Property

# hyphenationFactor

The threshold controlling when hyphenation is done.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedtvOS 9.0–13.0Deprecated

``` source
var hyphenationFactor: CGFloat { get set }
```

Deprecated

Use usesDefaultHyphenation instead.

## Discussion

Whenever (width of the real contents of the line) / (the line fragment width) is below `factor`, hyphenation is attempted when laying out the line. Hyphenation slows down text layout and increases memory usage, so it should be used sparingly.

## See Also

### Properties

attributedString

The text storage object from which the `NSGlyphGenerator` object procures characters for glyph generation.

layoutOptions

The layout manager’s current layout options.

var usesScreenFonts: Bool { get set }

A Boolean that controls using screen fonts to calculate layout and display text.

Deprecated

