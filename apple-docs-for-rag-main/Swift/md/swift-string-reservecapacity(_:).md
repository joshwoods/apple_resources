

- Swift
- String
-  reserveCapacity(\_:) 

Instance Method

# reserveCapacity(\_:)

Reserves enough space in the string’s underlying storage to store the specified number of ASCII characters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func reserveCapacity(_ n: Int)
```

## Parameters 

`n`  

The minimum number of ASCII character’s worth of storage to allocate.

## Discussion

Because each character in a string can require more than a single ASCII character’s worth of storage, additional allocation may be necessary when adding characters to a string after a call to `reserveCapacity(_:)`.

Complexity

O(*n*)

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

static func + (String, String) -> String

static func += (inout String, String)

static func + &lt;Other>(Other, Self) -> Self

Creates a new collection by concatenating the elements of a sequence and a collection.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of a collection and a sequence.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

