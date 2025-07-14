

- AppKit
- NSGlyphStorage
-  setIntAttribute(\_:value:forGlyphAt:) 

Instance Method

# setIntAttribute(\_:value:forGlyphAt:)

Sets a custom attribute value for a given glyph.

macOS

``` source
func setIntAttribute(
    _ attributeTag: Int,
    value val: Int,
    forGlyphAt glyphIndex: Int
)
```

**Required**

## Parameters 

`attributeTag`  

The custom attribute.

`val`  

The new attribute value.

`glyphIndex`  

Index of the glyph whose attribute is set.

## Discussion

Custom attributes are glyph attributes such as `NSGlyphInscription` or attributes defined by subclasses. Subclasses that define their own custom attributes must override this method and provide their own storage for the attribute values. Nonnegative tags are reserved; you can define your own attributes with negative tags and set values using this method.

## See Also

### Modifying the glyph cache

func insertGlyphs(UnsafePointer&lt;NSGlyph>, length: Int, forStartingGlyphAt: Int, characterIndex: Int)

Inserts the given glyphs into the glyph cache and maps them to the specified characters.

**Required**

