

- Core Text
-  CTFontDescriptorCreateCopyWithSymbolicTraits(\_:\_:\_:) 

Function

# CTFontDescriptorCreateCopyWithSymbolicTraits(\_:\_:\_:)

Creates a copy of the font descriptor with the specified symbolic traits as the original.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontDescriptorCreateCopyWithSymbolicTraits(
    _ original: CTFontDescriptor,
    _ symTraitValue: CTFontSymbolicTraits,
    _ symTraitMask: CTFontSymbolicTraits
) -> CTFontDescriptor?
```

## Parameters 

`original`  

The original font descriptor.

`symTraitValue`  

The value of the symbolic traits.

`symTraitMask`  

The mask bits of the symbolic traits. This parameter represents a bitfield that indicates which traits should be changed and which should be taken from the original font descriptor.

## Return Value

Returns a new font descriptor reference in the same family with the given symbolic traits, or `NULL` if no matching font descriptor is found in the system.

## Discussion

This bitfield of `symTraitValue` parameter indicates the desired value for the traits specified by the `symTraitMask` parameter. Used in conjunction, they can allow for trait removal as well as addition.

## See Also

### Creating Font Descriptors

func CTFontDescriptorCreateWithNameAndSize(CFString, CGFloat) -> CTFontDescriptor

Creates a new font descriptor with the provided PostScript name and size.

func CTFontDescriptorCreateWithAttributes(CFDictionary) -> CTFontDescriptor

Creates a new font descriptor reference from a dictionary of attributes.

func CTFontDescriptorCreateCopyWithAttributes(CTFontDescriptor, CFDictionary) -> CTFontDescriptor

Creates a copy of the original font descriptor with new attributes.

func CTFontDescriptorCreateCopyWithVariation(CTFontDescriptor, CFNumber, CGFloat) -> CTFontDescriptor

Creates a copy of the original font descriptor with a new variation instance.

func CTFontDescriptorCreateCopyWithFeature(CTFontDescriptor, CFNumber, CFNumber) -> CTFontDescriptor

Copies a font descriptor with new feature settings.

func CTFontDescriptorCreateCopyWithFamily(CTFontDescriptor, CFString) -> CTFontDescriptor?

Creates a copy of the font descriptor in the specified family based on the traits of the original.

func CTFontDescriptorCreateMatchingFontDescriptors(CTFontDescriptor, CFSet?) -> CFArray?

Returns an array of normalized font descriptors matching the provided descriptor.

func CTFontDescriptorCreateMatchingFontDescriptor(CTFontDescriptor, CFSet?) -> CTFontDescriptor?

Returns the single preferred matching font descriptor based on the original descriptor and system precedence.

