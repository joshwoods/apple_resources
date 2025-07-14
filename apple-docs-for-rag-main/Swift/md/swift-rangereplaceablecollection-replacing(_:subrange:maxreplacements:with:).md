

- Swift
- RangeReplaceableCollection
-  replacing(\_:subrange:maxReplacements:with:) 

Instance Method

# replacing(\_:subrange:maxReplacements:with:)

Returns a new collection in which all occurrences of a sequence matching the given regex are replaced by another regex match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacing(
    _ regex: some RegexComponent,
    subrange: Range,
    maxReplacements: Int = .max,
    with replacement: (Regex.Match) throws -> Replacement
) rethrows -> Self where Replacement : Collection, Replacement.Element == Character
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex describing the sequence to replace.

`subrange`  

The range in the collection in which to search for `regex`.

`maxReplacements`  

A number specifying how many occurrences of the sequence matching `regex` to replace. Default is `Int.max`.

`replacement`  

A closure that receives the full match information, including captures, and returns a replacement collection.

## Return Value

A new collection in which all occurrences of subsequence matching `regex` are replaced by `replacement`.

