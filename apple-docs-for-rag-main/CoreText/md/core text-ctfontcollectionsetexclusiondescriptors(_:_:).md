

- Core Text
-  CTFontCollectionSetExclusionDescriptors(\_:\_:) 

Function

# CTFontCollectionSetExclusionDescriptors(\_:\_:)

Replaces the array of descriptors to exclude from the match.

macOS 10.7+

``` source
func CTFontCollectionSetExclusionDescriptors(
    _ collection: CTMutableFontCollection,
    _ descriptors: CFArray?
)
```

## Parameters 

`collection`  

The font collection reference.

`descriptors`  

An array of CTFontDescriptor objects. This parameter can be `NULL`.

## See Also

### Excluding and Including Font Descriptors

func CTFontCollectionCopyExclusionDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors to exclude from the match.

func CTFontCollectionCopyQueryDescriptors(CTFontCollection) -> CFArray?

Retrieves the array of descriptors for font matching.

func CTFontCollectionSetQueryDescriptors(CTMutableFontCollection, CFArray?)

Replaces the array of descriptors for font matching.

