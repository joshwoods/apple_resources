

- Core Text
-  CTFontCollectionSortDescriptorsCallback 

Type Alias

# CTFontCollectionSortDescriptorsCallback

The collection sorting callback type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTFontCollectionSortDescriptorsCallback = (CTFontDescriptor, CTFontDescriptor, UnsafeMutableRawPointer) -> CFComparisonResult
```

## Parameters 

`first`  

The first descriptor.

`second`  

The second descriptor.

`refCon`  

A pointer to contextual data from the client.

## Return Value

The matching font descriptors of a collection in sorted order.

## See Also

### Getting Font Descriptors

func CTFontCollectionCreateMatchingFontDescriptors(CTFontCollection) -> CFArray?

Returns an array of font descriptors matching the collection.

func CTFontCollectionCreateMatchingFontDescriptorsWithOptions(CTFontCollection, CFDictionary?) -> CFArray?

Creates an array of font descriptors that match the specified collection.

func CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(CTFontCollection, CTFontCollectionSortDescriptorsCallback?, UnsafeMutableRawPointer?) -> CFArray?

Returns the array of matching font descriptors sorted with the callback function.

func CTFontCollectionCreateMatchingFontDescriptorsForFamily(CTFontCollection, CFString, CFDictionary?) -> CFArray?

Retrieves an array of font descriptors that match the specified family, one descriptor for each style in the collection.

