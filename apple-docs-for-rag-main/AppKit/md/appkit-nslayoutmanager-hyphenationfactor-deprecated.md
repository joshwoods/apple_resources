

- AppKit
- NSLayoutManager
-  hyphenationFactor Deprecated

Instance Property

# hyphenationFactor

The threshold controlling when hyphenation is done.

macOS 10.0–10.15Deprecated

``` source
var hyphenationFactor: Float { get set }
```

Deprecated

Use usesDefaultHyphenation instead.

## Discussion

Whenever (width of the real contents of the line) / (the line fragment width) is below `factor`, hyphenation is attempted when laying out the line. Hyphenation slows down text layout and increases memory usage, so it should be used sparingly.

## See Also

### Properties

var usesScreenFonts: Bool

A Boolean that controls using screen fonts to calculate layout and display text.

Deprecated

