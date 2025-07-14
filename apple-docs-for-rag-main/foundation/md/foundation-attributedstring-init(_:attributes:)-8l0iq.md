

- Foundation
- AttributedString
-  init(\_:attributes:) 

Initializer

# init(\_:attributes:)

Creates an attributed string from a character sequence and an attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ elements: S,
    attributes: AttributeContainer = .init()
) where S : Sequence, S.Element == Character
```

## Parameters 

`elements`  

A character sequence that provides the textual content for the attributed string.

`attributes`  

Attributes to apply to the textual content.

## See Also

### Creating an Attributed String

init()

Creates an empty attributed string.

init(AttributedSubstring)

Creates an attributed string from an attributed substring.

init(String, attributes: AttributeContainer)

Creates an attributed string from a string and an attribute container.

init(Substring, attributes: AttributeContainer)

Creates an attributed string from a substring and an attribute container.

struct AttributeContainer

A container for attribute keys and values.

