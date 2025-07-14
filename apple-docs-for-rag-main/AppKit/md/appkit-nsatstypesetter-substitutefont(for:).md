

- AppKit
- NSATSTypesetter
-  substituteFont(for:) 

Instance Method

# substituteFont(for:)

Returns a screen font suitable for use in place of the specified original font,.

macOS

``` source
func substituteFont(for originalFont: NSFont) -> NSFont
```

## Discussion

A screen font can be substituted if the receiver is set to use screen fonts and if no NSTextView associated with the receiver is scaled or rotated. If a suitable screen font isn’t available or usable, this method returns the original font.

