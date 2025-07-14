

- Swift
- RangeReplaceableCollection
-  replacing(\_:with:subrange:maxReplacements:) 

Instance Method

# replacing(\_:with:subrange:maxReplacements:)

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacing(
    _ regex: some RegexComponent,
    with replacement: Replacement,
    subrange: Range,
    maxReplacements: Int = .max
) -> Self where Replacement : Collection, Replacement.Element == Character
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex describing the sequence to replace.

`replacement`  

The new elements to add to the collection.

`subrange`  

The range in the collection in which to search for `regex`.

`maxReplacements`  

A number specifying how many occurrences of the sequence matching `regex` to replace. Default is `Int.max`.

## Return Value

A new collection in which all occurrences of subsequence matching `regex` in `subrange` are replaced by `replacement`.

