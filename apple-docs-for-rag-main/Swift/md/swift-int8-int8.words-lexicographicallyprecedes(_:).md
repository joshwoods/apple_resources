

- Swift
- Int8
- Int8.Words
-  lexicographicallyPrecedes(\_:) 

Instance Method

# lexicographicallyPrecedes(\_:)

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the less-than operator (`

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lexicographicallyPrecedes(_ other: OtherSequence) -> Bool where OtherSequence : Sequence, Self.Element == OtherSequence.Element
```

Available when `Element` conforms to `Comparable`.

## Parameters 

`other`  

A sequence to compare to this sequence.

## Return Value

`true` if this sequence precedes `other` in a dictionary ordering; otherwise, `false`.

## Discussion

This example uses the `lexicographicallyPrecedes` method to test which array of integers comes first in a lexicographical ordering.

```
let a = [1, 2, 2, 2]
let b = [1, 2, 3, 4]

print(a.lexicographicallyPrecedes(b))
// Prints "true"
print(b.lexicographicallyPrecedes(b))
// Prints "false"
```

Note

This method implements the mathematical notion of lexicographical ordering, which has no connection to Unicode. If you are sorting strings to present to the end user, use `String` APIs that perform localized comparison.

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `other`.

