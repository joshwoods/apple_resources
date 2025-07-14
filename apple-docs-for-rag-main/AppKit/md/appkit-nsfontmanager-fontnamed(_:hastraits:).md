

- AppKit
- NSFontManager
-  fontNamed(\_:hasTraits:) 

Instance Method

# fontNamed(\_:hasTraits:)

Indicates whether the given font has all the specified traits.

macOS

``` source
func fontNamed(
    _ fName: String,
    hasTraits someTraits: NSFontTraitMask
) -> Bool
```

## Parameters 

`fName`  

The name of the font.

`someTraits`  

The font traits to test, specified by combining the font trait mask values described in `Constants` using the C bitwise OR operator.

## Return Value

true if the font named `typeface` has all the traits specified in `fontTraitMask`; false if it doesn’t.

## Discussion

Using `NSUnboldFontMask` returns true if the font is not bold, false otherwise. Using `NSUnitalicFontMask` returns true if the font is not italic, false otherwise.

## See Also

### Examining Fonts

func traits(of: NSFont) -> NSFontTraitMask

Returns the traits of the given font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

func weight(of: NSFont) -> Int

Returns an approximation of the specified font’s weight.

