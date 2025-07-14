

- Foundation
- AttributedString
-  init(\_:including:) 

Initializer

# init(\_:including:)

Creates an attributed string from another attributed string, including an attribute scope that a key path identifies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ other: T,
    including scope: KeyPath
) where S : AttributeScope, T : AttributedStringProtocol
```

## Parameters 

`other`  

An attributed string or attributed substring.

`scope`  

An AttributeScopes key path that identifies an attribute scope to associate with the attributed string.

## See Also

### Creating a Duplicate Attributed String

init&lt;S, T>(T, including: S.Type)

Creates an attributed string from another attributed string, including an attribute scope.

