

- Swift
- String
-  insert(contentsOf:at:) 

Instance Method

# insert(contentsOf:at:)

Inserts a collection of characters at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func insert(
    contentsOf newElements: S,
    at i: String.Index
) where S : Collection, S.Element == Character
```

## Parameters 

`newElements`  

A collection of `Character` elements to insert into the string.

`i`  

A valid index of the string. If `i` is equal to the string’s end index, this methods appends the contents of `newElements` to the string.

## Discussion

Calling this method invalidates any existing indices for use with this string.

Complexity

O(*n*), where *n* is the combined length of the string and `newElements`.

## See Also

### Inserting Characters

func insert(Character, at: String.Index)

Inserts a new character at the specified position.

func insert(Self.Element, at: Self.Index)

Inserts a new element into the collection at the specified position.

func insert&lt;C>(contentsOf: C, at: Self.Index)

Inserts the elements of a sequence into the collection at the specified position.

