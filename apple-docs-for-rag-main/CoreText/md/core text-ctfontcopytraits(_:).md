

- Core Text
-  CTFontCopyTraits(\_:) 

Function

# CTFontCopyTraits(\_:)

Returns the traits dictionary of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyTraits(_ font: CTFont) -> CFDictionary
```

## Parameters 

`font`  

The font reference.

## Return Value

A retained reference to the font traits dictionary. Individual traits can be accessed with the trait key constants.

## Discussion

See the Constants section of CTFontDescriptor for a definition of the font traits.

## See Also

### Getting Font Data

func CTFontCopyFontDescriptor(CTFont) -> CTFontDescriptor

Returns the normalized font descriptor for the given font reference.

func CTFontCopyAttribute(CTFont, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute of the given font.

func CTFontGetSize(CTFont) -> CGFloat

Returns the point size of the given font.

func CTFontGetMatrix(CTFont) -> CGAffineTransform

Returns the transformation matrix of the given font.

func CTFontGetSymbolicTraits(CTFont) -> CTFontSymbolicTraits

Returns the symbolic traits of the given font.

func CTFontCopyDefaultCascadeListForLanguages(CTFont, CFArray?) -> CFArray?

Retrieves an ordered list of font substitution preferences.

