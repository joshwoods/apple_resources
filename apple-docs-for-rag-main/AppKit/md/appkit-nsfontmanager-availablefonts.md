

- AppKit
- NSFontManager
-  availableFonts 

Instance Property

# availableFonts

The names of the fonts available in the system (not the NSFont objects themselves).

macOS

``` source
var availableFonts: [String] { get }
```

## Discussion

Note that these fonts are in various system font directories.

## See Also

### Getting Available Fonts

var availableFontFamilies: [String]

The names of the font families available in the system.

func availableFontNames(with: NSFontTraitMask) -> [String]?

Returns the names of the fonts available in the system whose traits are described exactly by the given font trait mask (not the `NSFont` objects themselves).

func availableMembers(ofFontFamily: String) -> [[Any]]?

Returns an array with one entry for each available member of a font family.

