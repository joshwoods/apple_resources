

- Core Text
-  CTFontCollectionCopyFontAttribute(\_:\_:\_:) 

Function

# CTFontCollectionCopyFontAttribute(\_:\_:\_:)

Retrieves an array of font descriptor attribute values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.7+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func CTFontCollectionCopyFontAttribute(
    _ collection: CTFontCollection,
    _ attributeName: CFString,
    _ options: CTFontCollectionCopyOptions
) -> CFArray
```

## Parameters 

`collection`  

The font collection reference.

`attributeName`  

The attribute to retrieve for each descriptor in the collection.

`options`  

Options to alter the return value. With kCTFontCollectionCopyDefaultOptions, the values appear in the same order as the results from CTFontCollectionCreateMatchingFontDescriptors(_:), and `NULL` values transform to kCFNull. Setting unique removes duplicate values. Setting standardSort sorts the values in standard UI order.

## Return Value

An array that contains one value for each descriptor.

## See Also

### Get Font Descriptor Attributes

func CTFontCollectionCopyFontAttributes(CTFontCollection, CFSet, CTFontCollectionCopyOptions) -> CFArray

Retrieves an array of dictionaries containing font descriptor attribute values.

