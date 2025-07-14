

- AppKit
- NSFontManager
-  availableFontFamilies 

Instance Property

# availableFontFamilies

The names of the font families available in the system.

macOS

``` source
var availableFontFamilies: [String] { get }
```

## Discussion

Note that these fonts are in various system font directories.

## See Also

### Getting Available Fonts

var availableFonts: [String]

The names of the fonts available in the system (not the NSFont objects themselves).

func availableFontNames(with: NSFontTraitMask) -> [String]?

Returns the names of the fonts available in the system whose traits are described exactly by the given font trait mask (not the `NSFont` objects themselves).

func availableMembers(ofFontFamily: String) -> [[Any]]?

Returns an array with one entry for each available member of a font family.

