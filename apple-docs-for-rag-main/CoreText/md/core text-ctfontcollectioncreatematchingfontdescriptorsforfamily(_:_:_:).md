

- Core Text
-  CTFontCollectionCreateMatchingFontDescriptorsForFamily(\_:\_:\_:) 

Function

# CTFontCollectionCreateMatchingFontDescriptorsForFamily(\_:\_:\_:)

Retrieves an array of font descriptors that match the specified family, one descriptor for each style in the collection.

macOS 10.7+

``` source
func CTFontCollectionCreateMatchingFontDescriptorsForFamily(
    _ collection: CTFontCollection,
    _ familyName: CFString,
    _ options: CFDictionary?
) -> CFArray?
```

## Parameters 

`collection`  

The font collection reference.

`familyName`  

The font family name.

`options`  

The options dictionary.

## Return Value

An array of CTFontDescriptor objects that match the specified family in the collection, or `NULL` if there are none.

## See Also

### Getting Font Descriptors

func CTFontCollectionCreateMatchingFontDescriptors(CTFontCollection) -> CFArray?

Returns an array of font descriptors matching the collection.

func CTFontCollectionCreateMatchingFontDescriptorsWithOptions(CTFontCollection, CFDictionary?) -> CFArray?

Creates an array of font descriptors that match the specified collection.

func CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(CTFontCollection, CTFontCollectionSortDescriptorsCallback?, UnsafeMutableRawPointer?) -> CFArray?

Returns the array of matching font descriptors sorted with the callback function.

typealias CTFontCollectionSortDescriptorsCallback

The collection sorting callback type.

