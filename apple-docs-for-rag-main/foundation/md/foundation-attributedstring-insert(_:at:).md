

- Foundation
- AttributedString
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts the specified string at a specific index in the attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func insert(
    _ s: some AttributedStringProtocol,
    at index: AttributedString.Index
)
```

## Parameters 

`s`  

The string to insert.

`index`  

The index that indicates where to insert the string.

## See Also

### Modifying an Attributed String

struct Index

A type that represents the position of a character or code unit within an attributed string.

func removeSubrange(some RangeExpression&lt;AttributedString.Index>)

Removes a range of characters from the attributed string.

func replaceSubrange(some RangeExpression&lt;AttributedString.Index>, with: some AttributedStringProtocol)

Replaces the contents in a range of the attributed string.

