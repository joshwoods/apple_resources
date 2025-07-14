

- Swift
- String
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Creates a new collection by concatenating the elements of a collection and a sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func + (lhs: Self, rhs: Other) -> Self where Other : Sequence, Self.Element == Other.Element
```

## Parameters 

`lhs`  

A range-replaceable collection.

`rhs`  

A collection or finite sequence.

## Discussion

The two arguments must have the same `Element` type. For example, you can concatenate the elements of an integer array and a `Range` instance.

```
let numbers = [1, 2, 3, 4]
let moreNumbers = numbers + (5...10)
print(moreNumbers)
// Prints "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"
```

The resulting collection has the type of the argument on the left-hand side. In the example above, `moreNumbers` has the same type as `numbers`, which is `[Int]`.

## See Also

### Appending Strings and Characters

func append(String)

Appends the given string to this string.

func append(Character)

Appends the given character to the string.

func append(contentsOf: String)

func append(contentsOf: Substring)

func append&lt;S>(contentsOf: S)

Appends the characters in the given sequence to the string.

func append&lt;S>(contentsOf: S)

Adds the elements of a sequence or collection to the end of this collection.

func reserveCapacity(Int)

Reserves enough space in the string’s underlying storage to store the specified number of ASCII characters.

static func + (String, String) -> String

static func += (inout String, String)

static func + &lt;Other>(Other, Self) -> Self

Creates a new collection by concatenating the elements of a sequence and a collection.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

