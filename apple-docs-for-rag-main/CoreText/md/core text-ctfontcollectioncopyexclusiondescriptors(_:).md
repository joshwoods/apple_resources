

- Core Text
-  CTFontCollectionCopyExclusionDescriptors(\_:) 

Function

# CTFontCollectionCopyExclusionDescriptors(\_:)

Retrieves the array of descriptors to exclude from the match.

macOS 10.7+

``` source
func CTFontCollectionCopyExclusionDescriptors(_ collection: CTFontCollection) -> CFArray?
```

## Parameters 

`collection`  

The font collection reference.

## Return Value

A retained reference to the array of descriptors for querying (matching) the system font database.

## See Also

### Excluding and Including Font Descriptors

func CTFontCollectionCopyQueryDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors for font matching.

func CTFontCollectionSetExclusionDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors to exclude from the match.

func CTFontCollectionSetQueryDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors for font matching.

