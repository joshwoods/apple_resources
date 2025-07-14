

- Swift
- RangeReplaceableCollection
-  replace(maxReplacements:content:with:) 

Instance Method

# replace(maxReplacements:content:with:)

Replaces all matches for the regex in this collection, using the given closures to create the replacement and the regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func replace(
    maxReplacements: Int = .max,
    @RegexComponentBuilder content: () -> some RegexComponent,
    with replacement: (Regex.Match) throws -> Replacement
) rethrows where Replacement : Collection, Replacement.Element == Character
```

Available when `Self` conforms to `BidirectionalCollection` and `SubSequence` is `Substring`.

## Parameters 

`maxReplacements`  

A number specifying how many occurrences of the regex to replace, using `content` to create the regex.

`content`  

A closure that returns the collection to search for and replace.

`replacement`  

A closure that receives the full match information, including captures, and returns a replacement collection.

