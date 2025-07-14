

- Core Graphics
- CGFont
-  Font Variation Axis Keys 

API Collection

# Font Variation Axis Keys

Keys used for a font variation axis dictionary.

## Topics

### Constants

class let variationAxisName: CFString

The key used to obtain the variation axis name from a variation axis dictionary.

class let variationAxisMinValue: CFString

The key used to obtain the minimum variation axis value from a variation axis dictionary.

class let variationAxisMaxValue: CFString

The key used to obtain the maximum variation axis value from a variation axis dictionary.

class let variationAxisDefaultValue: CFString

The key used to obtain the default variation axis value from a variation axis dictionary.

## See Also

### Working with Variations

func copy(withVariations: CFDictionary?) -> CGFont?

Creates a copy of a font using a variation specification dictionary.

var variations: CFDictionary?

Returns the variation specification dictionary for a font.

var variationAxes: CFArray?

Returns an array of the variation axis dictionaries for a font.

