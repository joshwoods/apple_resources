

- Core Text
-  CTFontCollectionCreateMatchingFontDescriptors(\_:) 

Function

# CTFontCollectionCreateMatchingFontDescriptors(\_:)

Returns an array of font descriptors matching the collection.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCollectionCreateMatchingFontDescriptors(_ collection: CTFontCollection) -> CFArray?
```

## Parameters 

`collection`  

The font collection reference.

## Return Value

A retained reference to an array of normalized font descriptors matching the collection definition.

## See Also

### Getting Font Descriptors

func CTFontCollectionCreateMatchingFontDescriptorsWithOptions(CTFontCollection, CFDictionary?) -> CFArray?

Creates an array of font descriptors that match the specified collection.

func CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback(CTFontCollection, CTFontCollectionSortDescriptorsCallback?, UnsafeMutableRawPointer?) -> CFArray?

Returns the array of matching font descriptors sorted with the callback function.

func CTFontCollectionCreateMatchingFontDescriptorsForFamily(CTFontCollection, CFString, CFDictionary?) -> CFArray?

Retrieves an array of font descriptors that match the specified family, one descriptor for each style in the collection.

typealias CTFontCollectionSortDescriptorsCallback

The collection sorting callback type.

