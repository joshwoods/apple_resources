

- Swift
- Dictionary
-  init(\_:including:) 

Initializer

# init(\_:including:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ container: AttributeContainer,
    including scope: S.Type
) throws where S : AttributeScope
```

Available when `Key` is `NSAttributedString.Key` and `Value` is `Any`.

## See Also

### Creating a Dictionary from an Attribute Container

init&lt;S>(AttributeContainer, including: KeyPath&lt;AttributeScopes, S.Type>) throws

init(AttributeContainer)

