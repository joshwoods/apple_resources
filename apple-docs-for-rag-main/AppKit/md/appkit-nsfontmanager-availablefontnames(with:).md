

- AppKit
- NSFontManager
-  availableFontNames(with:) 

Instance Method

# availableFontNames(with:)

Returns the names of the fonts available in the system whose traits are described exactly by the given font trait mask (not the `NSFont` objects themselves).

macOS

``` source
func availableFontNames(with someTraits: NSFontTraitMask) -> [String]?
```

## Parameters 

`someTraits`  

The font traits for which to return font names. You specify the desired traits by combining the font trait mask values described in `Constants` using the C bitwise OR operator.

## Return Value

The names of the corresponding fonts.

## Discussion

These fonts are in various system font directories.

If `someTraits` is 0, this method returns all fonts that are neither italic nor bold. This result is the same one you’d get if `fontTraitMask` were `NSUnitalicFontMask` `|` `NSUnboldFontMask`.

## See Also

### Getting Available Fonts

var availableFonts: [String]

The names of the fonts available in the system (not the NSFont objects themselves).

var availableFontFamilies: [String]

The names of the font families available in the system.

func availableMembers(ofFontFamily: String) -> [[Any]]?

Returns an array with one entry for each available member of a font family.

