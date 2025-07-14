

- AppKit
- NSFontManager
-  weight(of:) 

Instance Method

# weight(of:)

Returns an approximation of the specified font’s weight.

macOS

``` source
func weight(of fontObj: NSFont) -> Int
```

## Parameters 

`fontObj`  

The font whose approximate weight is returned.

## Return Value

An approximation of the weight of the given font, where 0 indicates the lightest possible weight, 5 indicates a normal or book weight, and 9 or more indicates a bold or heavier weight. Because this method returns only an approximation of a font’s weight, it is not guaranteed to return the exact weight with which `fontObj` was initialized.

## See Also

### Examining Fonts

func traits(of: NSFont) -> NSFontTraitMask

Returns the traits of the given font.

func fontNamed(String, hasTraits: NSFontTraitMask) -> Bool

Indicates whether the given font has all the specified traits.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

