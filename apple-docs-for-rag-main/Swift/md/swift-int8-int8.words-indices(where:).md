

- Swift
- Int8
- Int8.Words
-  indices(where:) 

Instance Method

# indices(where:)

Returns the indices of all the elements that match the given predicate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func indices(where predicate: (Self.Element) throws -> Bool) rethrows -> RangeSet
```

## Parameters 

`predicate`  

A closure that takes an element as its argument and returns a Boolean value that indicates whether the passed element represents a match.

## Return Value

A set of the indices of the elements for which `predicate` returns `true`.

## Discussion

For example, you can use this method to find all the places that a vowel occurs in a string.

```
let str = "Fresh cheese in a breeze"
let vowels: Set = ["a", "e", "i", "o", "u"]
let allTheVowels = str.indices(where: { vowels.contains($0) })
// str[allTheVowels].count == 9
```

Complexity

O(*n*), where *n* is the length of the collection.

