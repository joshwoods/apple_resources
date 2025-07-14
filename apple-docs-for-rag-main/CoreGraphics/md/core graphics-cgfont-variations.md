

- Core Graphics
- CGFont
-  variations 

Instance Property

# variations

Returns the variation specification dictionary for a font.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var variations: CFDictionary? { get }
```

## Discussion

The variation specification dictionary contains keys that correspond to the variation axis names of the font. Each key is a variation axis name. The value for each key is the value specified for that particular variation axis represented as a doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd object.

## See Also

### Working with Variations

func copy(withVariations: CFDictionary?) -> CGFont?

Creates a copy of a font using a variation specification dictionary.

var variationAxes: CFArray?

Returns an array of the variation axis dictionaries for a font.

Font Variation Axis Keys

Keys used for a font variation axis dictionary.

