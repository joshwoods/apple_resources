

- Core Text
-  CTFontCollectionCreateMatchingFontDescriptorsWithOptions(\_:\_:) 

Function

# CTFontCollectionCreateMatchingFontDescriptorsWithOptions(\_:\_:)

Creates an array of font descriptors that match the specified collection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.7+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func CTFontCollectionCreateMatchingFontDescriptorsWithOptions(
    _ collection: CTFontCollection,
    _ options: CFDictionary?
) -> CFArray?
```

## Parameters 

`collection`  

The font collection reference.

`options`  

The options dictionary. Passing in `NULL` returns the same results as calling CTFontCollectionCreateMatchingFontDescriptors(_:), which uses the options specified during the collection’s creation.

## Return Value

An array of CTFontDescriptor objects that match the collection definition, or `NULL` if there are none.

## See Also

### Getting Font Descriptors

func CTFontCollectionCreateMatchingFontDescriptors(CTFontCollection) -> CFArray?

Returns an array of font descriptors matching the collection.

func CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(CTFontCollection, CTFontCollectionSortDescriptorsCallback?, UnsafeMutableRawPointer?) -> CFArray?

Returns the array of matching font descriptors sorted with the callback function.

func CTFontCollectionCreateMatchingFontDescriptorsForFamily(CTFontCollection, CFString, CFDictionary?) -> CFArray?

Retrieves an array of font descriptors that match the specified family, one descriptor for each style in the collection.

typealias CTFontCollectionSortDescriptorsCallback

The collection sorting callback type.

