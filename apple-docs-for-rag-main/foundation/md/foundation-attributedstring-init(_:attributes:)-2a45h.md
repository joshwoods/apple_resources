

- Foundation
- AttributedString
-  init(\_:attributes:) 

Initializer

# init(\_:attributes:)

Creates an attributed string from a string and an attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ string: String,
    attributes: AttributeContainer = .init()
)
```

## Parameters 

`string`  

A string to add attributes to.

`attributes`  

Attributes to apply to `string`.

## See Also

### Creating an Attributed String

init()

Creates an empty attributed string.

init(AttributedSubstring)

Creates an attributed string from an attributed substring.

init(Substring, attributes: AttributeContainer)

Creates an attributed string from a substring and an attribute container.

init&lt;S>(S, attributes: AttributeContainer)

Creates an attributed string from a character sequence and an attribute container.

struct AttributeContainer

A container for attribute keys and values.

