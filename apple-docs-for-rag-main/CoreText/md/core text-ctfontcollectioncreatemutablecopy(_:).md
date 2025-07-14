

- Core Text
-  CTFontCollectionCreateMutableCopy(\_:) 

Function

# CTFontCollectionCreateMutableCopy(\_:)

Creates a mutable copy of the original collection.

macOS 10.7+

``` source
func CTFontCollectionCreateMutableCopy(_ original: CTFontCollection) -> CTMutableFontCollection
```

## Parameters 

`original`  

The original font collection reference.

## Return Value

A mutable copy of the original font collection.

## See Also

### Creating Font Collections

func CTFontCollectionCreateFromAvailableFonts(CFDictionary?) -> CTFontCollection

Returns a new font collection containing all available fonts.

func CTFontCollectionCreateWithFontDescriptors(CFArray?, CFDictionary?) -> CTFontCollection

Returns a new font collection based on the given array of font descriptors.

func CTFontCollectionCreateCopyWithFontDescriptors(CTFontCollection, CFArray?, CFDictionary?) -> CTFontCollection

Returns a copy of the original collection augmented with the given new font descriptors.

