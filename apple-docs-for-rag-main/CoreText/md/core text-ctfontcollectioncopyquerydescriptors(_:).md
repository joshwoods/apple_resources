

- Core Text
-  CTFontCollectionCopyQueryDescriptors(\_:) 

Function

# CTFontCollectionCopyQueryDescriptors(\_:)

Retrieves the array of descriptors for font matching.

macOS 10.7+

``` source
func CTFontCollectionCopyQueryDescriptors(_ collection: CTFontCollection) -> CFArray?
```

## Parameters 

`collection`  

The font collection reference.

## Return Value

A retained reference to the array of descriptors for querying (matching) the system font database. The return value is undefined if you create the collection with CTFontCollectionCreateFromAvailableFonts(_:).

## See Also

### Excluding and Including Font Descriptors

func CTFontCollectionCopyExclusionDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors to exclude from the match.

func CTFontCollectionSetExclusionDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors to exclude from the match.

func CTFontCollectionSetQueryDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors for font matching.

