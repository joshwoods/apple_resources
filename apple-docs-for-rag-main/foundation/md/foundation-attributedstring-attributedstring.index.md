

- Foundation
- AttributedString
-  AttributedString.Index 

Structure

# AttributedString.Index

A type that represents the position of a character or code unit within an attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Index
```

## Topics

### Initializers

init?&lt;S>(String.Index, within: S)

## Relationships

### Conforms To

- Comparable
- Equatable
- Sendable

## See Also

### Modifying an Attributed String

func insert(some AttributedStringProtocol, at: AttributedString.Index)

Inserts the specified string at a specific index in the attributed string.

func removeSubrange(some RangeExpression&lt;AttributedString.Index>)

Removes a range of characters from the attributed string.

func replaceSubrange(some RangeExpression&lt;AttributedString.Index>, with: some AttributedStringProtocol)

Replaces the contents in a range of the attributed string.

