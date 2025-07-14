

- Core Text
-  CTFontGetSize(\_:) 

Function

# CTFontGetSize(\_:)

Returns the point size of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetSize(_ font: CTFont) -> CGFloat
```

## Parameters 

`font`  

The font reference.

## Return Value

The point size of the given font reference. This is the point size provided when the font was created.

## See Also

### Getting Font Data

func CTFontCopyFontDescriptor(CTFont) -> CTFontDescriptor

Returns the normalized font descriptor for the given font reference.

func CTFontCopyAttribute(CTFont, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute of the given font.

func CTFontGetMatrix(CTFont) -> CGAffineTransform

Returns the transformation matrix of the given font.

func CTFontGetSymbolicTraits(CTFont) -> CTFontSymbolicTraits

Returns the symbolic traits of the given font.

func CTFontCopyTraits(CTFont) -> CFDictionary

Returns the traits dictionary of the given font.

func CTFontCopyDefaultCascadeListForLanguages(CTFont, CFArray?) -> CFArray?

Retrieves an ordered list of font substitution preferences.

