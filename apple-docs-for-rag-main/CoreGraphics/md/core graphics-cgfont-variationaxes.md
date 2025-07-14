

- Core Graphics
- CGFont
-  variationAxes 

Instance Property

# variationAxes

Returns an array of the variation axis dictionaries for a font.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var variationAxes: CFArray? { get }
```

## Discussion

A variation axis is a range included in a font by the font designer that allows a font to produce different type styles. Each variation axis dictionary contains key-value pairs that specify the variation axis name and the minimum, maximum, and default values for that variation axis.

## See Also

### Working with Variations

func copy(withVariations: CFDictionary?) -> CGFont?

Creates a copy of a font using a variation specification dictionary.

var variations: CFDictionary?

Returns the variation specification dictionary for a font.

Font Variation Axis Keys

Keys used for a font variation axis dictionary.

