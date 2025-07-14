

- Swift
- Array
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Adds the elements of a sequence to the end of the array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func append(contentsOf newElements: S) where Element == S.Element, S : Sequence
```

## Parameters 

`newElements`  

The elements to append to the array.

## Discussion

Use this method to append the elements of a sequence to the end of this array. This example appends the elements of a `Range` instance to an array of integers.

```
var numbers = [1, 2, 3, 4, 5]
numbers.append(contentsOf: 10...15)
print(numbers)
// Prints "[1, 2, 3, 4, 5, 10, 11, 12, 13, 14, 15]"
```

Complexity

O(*m*) on average, where *m* is the length of `newElements`, over many calls to `append(contentsOf:)` on the same array.

## See Also

### Combining Arrays

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

static func + &lt;Other>(Other, Self) -> Self

Creates a new collection by concatenating the elements of a sequence and a collection.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of a collection and a sequence.

static func + (Array&lt;Element>, Array&lt;Element>) -> Array&lt;Element>

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

static func += (inout Array&lt;Element>, Array&lt;Element>)

