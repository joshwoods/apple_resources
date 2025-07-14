

- Core Text
-  CTFontCollectionCreateFromAvailableFonts(\_:) 

Function

# CTFontCollectionCreateFromAvailableFonts(\_:)

Returns a new font collection containing all available fonts.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCollectionCreateFromAvailableFonts(_ options: CFDictionary?) -> CTFontCollection
```

## Parameters 

`options`  

The options dictionary. For possible values, see Constants.

## Return Value

A new collection containing all fonts available to the current application.

## See Also

### Creating Font Collections

func CTFontCollectionCreateWithFontDescriptors(CFArray?, CFDictionary?) -> CTFontCollection

Returns a new font collection based on the given array of font descriptors.

func CTFontCollectionCreateCopyWithFontDescriptors(CTFontCollection, CFArray?, CFDictionary?) -> CTFontCollection

Returns a copy of the original collection augmented with the given new font descriptors.

func CTFontCollectionCreateMutableCopy(CTFontCollection) -> CTMutableFontCollection

Creates a mutable copy of the original collection.

