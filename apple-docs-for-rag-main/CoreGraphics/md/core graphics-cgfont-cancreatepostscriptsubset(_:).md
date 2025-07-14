

- Core Graphics
- CGFont
-  canCreatePostScriptSubset(\_:) 

Instance Method

# canCreatePostScriptSubset(\_:)

Determines whether Core Graphics can create a subset of the font in PostScript format.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func canCreatePostScriptSubset(_ format: CGFontPostScriptFormat) -> Bool
```

## Parameters 

`format`  

A PostScript font format.

## Return Value

Returns `true` if a subset in the PostScript format can be created for the font; `false` otherwise.

## Discussion

For more information on PostScript format, see *Adobe Type 1 Font Format*, which is available from http://partners.adobe.com/.

## See Also

### Working with PostScript Fonts

var postScriptName: CFString?

Obtains the PostScript name of a font.

func createPostScriptSubset(subsetName: CFString, format: CGFontPostScriptFormat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int, encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a subset of the font in the specified PostScript format.

enum CGFontPostScriptFormat

Possible formats for a PostScript font subset.

func createPostScriptEncoding(encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a PostScript encoding of a font.

