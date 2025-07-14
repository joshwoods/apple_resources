

- Core Text
-  CTFontCollectionCopyFontAttributes(\_:\_:\_:) 

Function

# CTFontCollectionCopyFontAttributes(\_:\_:\_:)

Retrieves an array of dictionaries containing font descriptor attribute values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.7+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func CTFontCollectionCopyFontAttributes(
    _ collection: CTFontCollection,
    _ attributeNames: CFSet,
    _ options: CTFontCollectionCopyOptions
) -> CFArray
```

## Parameters 

`collection`  

The font collection reference.

`attributeNames`  

The attributes to retrieve for each descriptor in the collection.

`options`  

Options to alter the return value. With kCTFontCollectionCopyDefaultOptions, the values appear in the same order as the results from CTFontCollectionCreateMatchingFontDescriptors(_:). Setting unique removes duplicate values. Setting standardSort sorts the values in standard UI order.

## Return Value

An array that contains one CFDictionary value for each descriptor mapping the specified attribute names.

## See Also

### Get Font Descriptor Attributes

func CTFontCollectionCopyFontAttribute(CTFontCollection, CFString, CTFontCollectionCopyOptions) -> CFArray

Retrieves an array of font descriptor attribute values.

