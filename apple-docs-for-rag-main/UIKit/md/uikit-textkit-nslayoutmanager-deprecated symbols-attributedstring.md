

- UIKit
- TextKit
- NSLayoutManager
- Deprecated symbols
-  attributedString 

Article

# attributedString

The text storage object from which the `NSGlyphGenerator` object procures characters for glyph generation.

## Overview

- Swift
- Objective-C

```
var attributedString: NSAttributedString? { get }
```

```
@property(readonly, strong) NSAttributedString *attributedString
```

This property is part of the `NSGlyphStorage` protocol, for use by the glyph generator. For `NSLayoutManager` the attributed string is equivalent to the text storage.

## See Also

### Properties

var hyphenationFactor: CGFloat

The threshold controlling when hyphenation is done.

Deprecated

layoutOptions

The layout manager’s current layout options.

var usesScreenFonts: Bool { get set }

A Boolean that controls using screen fonts to calculate layout and display text.

Deprecated

