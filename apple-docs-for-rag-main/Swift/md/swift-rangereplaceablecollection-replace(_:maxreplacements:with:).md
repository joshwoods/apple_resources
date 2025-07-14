

- Swift
- RangeReplaceableCollection
-  replace(\_:maxReplacements:with:) 

Instance Method

# replace(\_:maxReplacements:with:)

Replaces all occurrences of the sequence matching the given regex with a given collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func replace(
    _ regex: some RegexComponent,
    maxReplacements: Int = .max,
    with replacement: (Regex.Match) throws -> Replacement
) rethrows where Replacement : Collection, Replacement.Element == Character
```

Available when `SubSequence` is `Substring`.

## Parameters 

`regex`  

A regex describing the sequence to replace.

`maxReplacements`  

A number specifying how many occurrences of the sequence matching `regex` to replace. Default is `Int.max`.

`replacement`  

A closure that receives the full match information, including captures, and returns a replacement collection.

