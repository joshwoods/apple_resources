

- Core Text
-  CTFontCollectionCreateWithFontDescriptors(\_:\_:) 

Function

# CTFontCollectionCreateWithFontDescriptors(\_:\_:)

Returns a new font collection based on the given array of font descriptors.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCollectionCreateWithFontDescriptors(
    _ queryDescriptors: CFArray?,
    _ options: CFDictionary?
) -> CTFontCollection
```

## Parameters 

`queryDescriptors`  

An array of font descriptors.

`options`  

The options dictionary. For possible values, see Constants.

## Return Value

A new font collection based on the provided font descriptors.

## Discussion

The contents of the returned collection are defined by matching the provided descriptors against all available font descriptors.

## See Also

### Creating Font Collections

func CTFontCollectionCreateFromAvailableFonts(CFDictionary?) -> CTFontCollection

Returns a new font collection containing all available fonts.

func CTFontCollectionCreateCopyWithFontDescriptors(CTFontCollection, CFArray?, CFDictionary?) -> CTFontCollection

Returns a copy of the original collection augmented with the given new font descriptors.

func CTFontCollectionCreateMutableCopy(CTFontCollection) -> CTMutableFontCollection

Creates a mutable copy of the original collection.

