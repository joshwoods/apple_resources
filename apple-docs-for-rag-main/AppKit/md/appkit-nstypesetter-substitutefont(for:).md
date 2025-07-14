

- AppKit
- NSTypesetter
-  substituteFont(for:) 

Instance Method

# substituteFont(for:)

Returns a screen font suitable for use in place of a given font.

macOS

``` source
func substituteFont(for originalFont: NSFont) -> NSFont
```

## Parameters 

`originalFont`  

The original font.

## Return Value

A screen font suitable for use in place of `originalFont`. This method returns `originalFont` if a screen font can’t be used or isn’t available.

## Discussion

A screen font can only be substituted if the receiver is set to use screen fonts and if no text view associated with the receiver is scaled or rotated.

