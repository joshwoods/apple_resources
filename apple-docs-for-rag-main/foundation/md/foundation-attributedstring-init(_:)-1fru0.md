

- Foundation
- AttributedString
-  init(\_:) 

Initializer

# init(\_:)

Creates a value-type attributed string from a reference type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ nsStr: NSAttributedString)
```

## Parameters 

`nsStr`  

The NSAttributedString to convert.

## Discussion

This initializer includes all attribute scopes defined by the SDK, such as AttributeScopes.FoundationAttributes, AttributeScopes.SwiftUIAttributes, and AttributeScopes.AccessibilityAttributes. To use third-party attribute scopes, use the initializers init(_:including:) or init(_:including:).

## See Also

### Creating an Attributed String from a Reference Type

init&lt;S>(NSAttributedString, including: S.Type) throws

Creates a value-type attributed string from a reference type, including an attribute scope.

init&lt;S>(NSAttributedString, including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates a value-type attributed string from a reference type, including an attribute scope that a key path identifies.

