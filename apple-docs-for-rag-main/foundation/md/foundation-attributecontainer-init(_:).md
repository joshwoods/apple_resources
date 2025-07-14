

- Foundation
- AttributeContainer
-  init(\_:) 

Initializer

# init(\_:)

Creates an attribute container from a dictionary, using default attribute scopes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ dictionary: [NSAttributedString.Key : Any])
```

## Parameters 

`dictionary`  

A dictionary of attribute keys and their values.

## Discussion

This initializer includes all attribute scopes defined by the SDK, such as AttributeScopes.FoundationAttributes, AttributeScopes.SwiftUIAttributes, and AttributeScopes.AccessibilityAttributes. To use third-party attribute scopes, use the initializers init(_:including:) and init(_:including:).

## See Also

### Creating an Attribute Container

init()

Creates an empty attribute container.

init&lt;S>([NSAttributedString.Key : Any], including: S.Type) throws

Creates an attribute container from a dictionary and an attribute scope.

init&lt;S>([NSAttributedString.Key : Any], including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates an attribute container from a dictionary and an attribute scope that a key path identifies.

