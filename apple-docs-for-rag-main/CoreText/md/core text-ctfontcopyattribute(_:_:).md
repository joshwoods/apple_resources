

- Core Text
-  CTFontCopyAttribute(\_:\_:) 

Function

# CTFontCopyAttribute(\_:\_:)

Returns the value associated with an arbitrary attribute of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyAttribute(
    _ font: CTFont,
    _ attribute: CFString
) -> CFTypeRef?
```

## Parameters 

`font`  

The font reference.

`attribute`  

The requested attribute.

## Return Value

A retained reference to an arbitrary attribute or `NULL` if the requested attribute is not present.

## Discussion

Refer to the attribute definitions documentation for information as to how each attribute is packaged as a `CFType`.

## See Also

### Getting Font Data

func CTFontCopyFontDescriptor(CTFont) -> CTFontDescriptor

Returns the normalized font descriptor for the given font reference.

func CTFontGetSize(CTFont) -> CGFloat

Returns the point size of the given font.

func CTFontGetMatrix(CTFont) -> CGAffineTransform

Returns the transformation matrix of the given font.

func CTFontGetSymbolicTraits(CTFont) -> CTFontSymbolicTraits

Returns the symbolic traits of the given font.

func CTFontCopyTraits(CTFont) -> CFDictionary

Returns the traits dictionary of the given font.

func CTFontCopyDefaultCascadeListForLanguages(CTFont, CFArray?) -> CFArray?

Retrieves an ordered list of font substitution preferences.

