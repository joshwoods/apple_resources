

- Foundation
- NSAttributedString
-  init(\_:) 

Initializer

# init(\_:)

Creates a reference-type attributed string from the specified value-type attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(_ attrStr: AttributedString)
```

## Parameters 

`attrStr`  

The value type attributed string that provides the text and attributes of the new object.

## Discussion

This initializer includes all attribute scopes defined by the SDK, such as AttributeScopes.FoundationAttributes, AttributeScopes.SwiftUIAttributes, and AttributeScopes.AccessibilityAttributes. To use third-party attribute scopes, use the initializers init(_:including:) or init(_:including:).

## See Also

### Creating a formatted string

convenience init&lt;S>(AttributedString, including: S.Type) throws

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope.

convenience init&lt;S>(AttributedString, including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope that a key path identifies.

