

- Core Text
-  CTFontCollectionSetQueryDescriptors(\_:\_:) 

Function

# CTFontCollectionSetQueryDescriptors(\_:\_:)

Replaces the array of descriptors for font matching.

macOS 10.7+

``` source
func CTFontCollectionSetQueryDescriptors(
    _ collection: CTMutableFontCollection,
    _ descriptors: CFArray?
)
```

## Parameters 

`collection`  

The font collection reference.

`descriptors`  

An array of CTFontDescriptor objects. Passing in `NULL` represents an empty collection, which sets the matching descriptors to `NULL`.

## See Also

### Excluding and Including Font Descriptors

func CTFontCollectionCopyExclusionDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors to exclude from the match.

func CTFontCollectionCopyQueryDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors for font matching.

func CTFontCollectionSetExclusionDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors to exclude from the match.

