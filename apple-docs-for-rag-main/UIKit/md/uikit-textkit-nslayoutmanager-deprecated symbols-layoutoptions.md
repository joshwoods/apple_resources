

- UIKit
- TextKit
- NSLayoutManager
- Deprecated symbols
-  layoutOptions 

Article

# layoutOptions

The layout manager’s current layout options.

## Overview

- Swift
- Objective-C

```
var layoutOptions: Int { get }
```

```
@property(readonly) NSUInteger layoutOptions
```

This property is part of the `NSGlyphStorage` protocol, for use by the glyph generator. It enables the glyph generator to ask which options the layout manager requests.

## See Also

### Properties

var hyphenationFactor: CGFloat

The threshold controlling when hyphenation is done.

Deprecated

attributedString

The text storage object from which the `NSGlyphGenerator` object procures characters for glyph generation.

var usesScreenFonts: Bool { get set }

A Boolean that controls using screen fonts to calculate layout and display text.

Deprecated

