

- Core Text
-  CTFontDescriptorCreateCopyWithFeature(\_:\_:\_:) 

Function

# CTFontDescriptorCreateCopyWithFeature(\_:\_:\_:)

Copies a font descriptor with new feature settings.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontDescriptorCreateCopyWithFeature(
    _ original: CTFontDescriptor,
    _ featureTypeIdentifier: CFNumber,
    _ featureSelectorIdentifier: CFNumber
) -> CTFontDescriptor
```

## Parameters 

`original`  

The original font descriptor.

`featureTypeIdentifier`  

The feature type identifier.

`featureSelectorIdentifier`  

The feature selector identifier.

## Return Value

A copy of the original font descriptor modified with the given feature settings.

## Discussion

This is a convenience method to toggle more easily the state of individual features.

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

func CTFontDescriptorCreateCopyWithFamily(CTFontDescriptor, CFString) -> CTFontDescriptor?

Creates a copy of the font descriptor in the specified family based on the traits of the original.

func CTFontDescriptorCreateCopyWithSymbolicTraits(CTFontDescriptor, CTFontSymbolicTraits, CTFontSymbolicTraits) -> CTFontDescriptor?

Creates a copy of the font descriptor with the specified symbolic traits as the original.

func CTFontDescriptorCreateMatchingFontDescriptors(CTFontDescriptor, CFSet?) -> CFArray?

Returns an array of normalized font descriptors matching the provided descriptor.

func CTFontDescriptorCreateMatchingFontDescriptor(CTFontDescriptor, CFSet?) -> CTFontDescriptor?

Returns the single preferred matching font descriptor based on the original descriptor and system precedence.

