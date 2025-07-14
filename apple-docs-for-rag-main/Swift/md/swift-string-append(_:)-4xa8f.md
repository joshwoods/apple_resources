

- Swift
- String
-  append(\_:) 

Instance Method

# append(\_:)

Appends the given string to this string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func append(_ other: String)
```

## Parameters 

`other`  

Another string.

## Discussion

The following example builds a customized greeting by using the `append(_:)` method:

```
var greeting = "Hello, "
if let name = getUserName() {
    greeting.append(name)
} else {
    greeting.append("friend")
}
print(greeting)
// Prints "Hello, friend"
```

## See Also

### Appending Strings and Characters

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

Creates a new collection by concatenating the elements of a collection and a sequence.

static func + &lt;Other>(Self, Other) -> Self

Creates a new collection by concatenating the elements of two collections.

static func += &lt;Other>(inout Self, Other)

Appends the elements of a sequence to a range-replaceable collection.

