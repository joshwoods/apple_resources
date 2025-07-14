

- Swift
- RangeReplaceableCollection
-  replacing(subrange:maxReplacements:content:with:) 

Instance Method

# replacing(subrange:maxReplacements:content:with:)

Returns a new collection in which all matches for the regex are replaced, using the given closures to create the replacement and the regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacing(
    subrange: Range,
    maxReplacements: Int = .max,
    @RegexComponentBuilder content: () -> some RegexComponent,
    with replacement: (Regex.Match) throws -> Replacement
) rethrows -> Self where Replacement : Collection, Replacement.Element == Character
```

Available when `Self` conforms to `BidirectionalCollection` and `SubSequence` is `Substring`.

## Parameters 

`subrange`  

The range in the collection in which to search for the regex, using `content` to create the regex.

`maxReplacements`  

A number specifying how many occurrences of the regex to replace.

`content`  

A closure that returns the collection to search for and replace.

`replacement`  

A closure that receives the full match information, including captures, and returns a replacement collection.

## Return Value

A new collection in which all matches for regex in `subrange` are replaced by the result of calling `replacement`, where regex is the result of calling `content`.

