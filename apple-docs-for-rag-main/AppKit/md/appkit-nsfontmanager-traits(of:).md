

- AppKit
- NSFontManager
-  traits(of:) 

Instance Method

# traits(of:)

Returns the traits of the given font.

macOS

``` source
func traits(of fontObj: NSFont) -> NSFontTraitMask
```

## Parameters 

`fontObj`  

The font whose traits are returned.

## Return Value

The font traits, returned as a mask created by combining values listed in `Constants` with the C bitwise OR operator.

## See Also

### Examining Fonts

func fontNamed(String, hasTraits: NSFontTraitMask) -> Bool

Indicates whether the given font has all the specified traits.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

func weight(of: NSFont) -> Int

Returns an approximation of the specified font’s weight.

