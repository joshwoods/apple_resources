

- Core Text
-  CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(\_:\_:\_:) 

Function

# CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(\_:\_:\_:)

Returns the array of matching font descriptors sorted with the callback function.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(
    _ collection: CTFontCollection,
    _ sortCallback: CTFontCollectionSortDescriptorsCallback?,
    _ refCon: UnsafeMutableRawPointer?
) -> CFArray?
```

## Parameters 

`collection`  

The collection reference.

`sortCallback`  

The sorting callback function that defines the sort order.

`refCon`  

Pointer to client data define context for the callback.

## Return Value

An array of font descriptors matching the criteria of the collection sorted by the results of the sorting callback function.

## See Also

### Getting Font Descriptors

func CTFontCollectionCreateMatchingFontDescriptors(CTFontCollection) -> CFArray?

Returns an array of font descriptors matching the collection.

func CTFontCollectionCreateMatchingFontDescriptorsWithOptions(CTFontCollection, CFDictionary?) -> CFArray?

Creates an array of font descriptors that match the specified collection.

func CTFontCollectionCreateMatchingFontDescriptorsForFamily(CTFontCollection, CFString, CFDictionary?) -> CFArray?

Retrieves an array of font descriptors that match the specified family, one descriptor for each style in the collection.

typealias CTFontCollectionSortDescriptorsCallback

The collection sorting callback type.

