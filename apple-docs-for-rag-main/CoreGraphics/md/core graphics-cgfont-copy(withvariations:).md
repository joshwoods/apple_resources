

- Core Graphics
- CGFont
-  copy(withVariations:) 

Instance Method

# copy(withVariations:)

Creates a copy of a font using a variation specification dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func copy(withVariations variations: CFDictionary?) -> CGFont?
```

## Parameters 

`variations`  

A variation specification dictionary that contains keys corresponding to the variation axis names of the font. Each key in the dictionary is a variation axis name. The value for each key is the value specified for that particular variation axis represented as a CFNumber object. If a variation axis name is not specified in `variations`, then the current value from `font` is used.

## Return Value

The font object.

## See Also

### Working with Variations

var variations: CFDictionary?

Returns the variation specification dictionary for a font.

var variationAxes: CFArray?

Returns an array of the variation axis dictionaries for a font.

Font Variation Axis Keys

Keys used for a font variation axis dictionary.

