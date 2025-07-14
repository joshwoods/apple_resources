

- Core Graphics
- CGFont
-  createPostScriptSubset(subsetName:format:glyphs:count:encoding:) 

Instance Method

# createPostScriptSubset(subsetName:format:glyphs:count:encoding:)

Creates a subset of the font in the specified PostScript format.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func createPostScriptSubset(
    subsetName: CFString,
    format: CGFontPostScriptFormat,
    glyphs: UnsafePointer?,
    count: Int,
    encoding: UnsafePointer?
) -> CFData?
```

## Parameters 

`subsetName`  

The name of the subset.

`format`  

The PostScript format of the font.

`glyphs`  

An array that contains the glyphs in the subset.

`count`  

The number of glyphs specified by the `glyphs` array.

`encoding`  

The default encoding for the subset. You can pass `nil` if you do not want to specify an encoding.

## Return Value

A subset of the font created from the supplied parameters.

## Discussion

For more information on PostScript format, see *Adobe Type 1 Font Format*, which is available from http://partners.adobe.com/.

## See Also

### Working with PostScript Fonts

var postScriptName: CFString?

Obtains the PostScript name of a font.

func canCreatePostScriptSubset(CGFontPostScriptFormat) -> Bool

Determines whether Core Graphics can create a subset of the font in PostScript format.

enum CGFontPostScriptFormat

Possible formats for a PostScript font subset.

func createPostScriptEncoding(encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a PostScript encoding of a font.

