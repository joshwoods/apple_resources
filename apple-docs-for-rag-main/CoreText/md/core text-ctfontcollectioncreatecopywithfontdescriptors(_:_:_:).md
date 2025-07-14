

- Core Text
-  CTFontCollectionCreateCopyWithFontDescriptors(\_:\_:\_:) 

Function

# CTFontCollectionCreateCopyWithFontDescriptors(\_:\_:\_:)

Returns a copy of the original collection augmented with the given new font descriptors.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCollectionCreateCopyWithFontDescriptors(
    _ original: CTFontCollection,
    _ queryDescriptors: CFArray?,
    _ options: CFDictionary?
) -> CTFontCollection
```

## Parameters 

`original`  

The original font collection reference.

`queryDescriptors`  

An array of font descriptors to augment those of the original collection.

`options`  

The options dictionary. For possible values, see Constants.

## Return Value

A copy of the original font collection augmented by the new font descriptors and options.

## Discussion

The new font descriptors are merged with the existing descriptors to create a single set.

## See Also

### Creating Font Collections

func CTFontCollectionCreateFromAvailableFonts(CFDictionary?) -> CTFontCollection

Returns a new font collection containing all available fonts.

func CTFontCollectionCreateWithFontDescriptors(CFArray?, CFDictionary?) -> CTFontCollection

Returns a new font collection based on the given array of font descriptors.

func CTFontCollectionCreateMutableCopy(CTFontCollection) -> CTMutableFontCollection

Creates a mutable copy of the original collection.

