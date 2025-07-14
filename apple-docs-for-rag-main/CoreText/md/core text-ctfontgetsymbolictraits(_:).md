

- Core Text
-  CTFontGetSymbolicTraits(\_:) 

Function

# CTFontGetSymbolicTraits(\_:)

Returns the symbolic traits of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetSymbolicTraits(_ font: CTFont) -> CTFontSymbolicTraits
```

## Parameters 

`font`  

The font reference.

## Return Value

The symbolic traits of the font. This is equivalent to the `kCTFontSymbolicTrait` value of the traits dictionary.

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

func CTFontCopyTraits(CTFont) -> CFDictionary

Returns the traits dictionary of the given font.

func CTFontCopyDefaultCascadeListForLanguages(CTFont, CFArray?) -> CFArray?

Retrieves an ordered list of font substitution preferences.

