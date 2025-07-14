

- Foundation
- AttributeContainer
-  init(\_:including:) 

Initializer

# init(\_:including:)

Creates an attribute container from a dictionary and an attribute scope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ dictionary: [NSAttributedString.Key : Any],
    including scope: S.Type
) throws where S : AttributeScope
```

## Parameters 

`dictionary`  

A dictionary of attribute keys and their values.

`scope`  

The attribute scope of the dictionary keys. This can be a nested scope that contains several scopes.

## Discussion

This initializer only collects attributes from `dictionary` that exist in the provided scope. The resulting attribute container omits any keys in `dictionary` that don’t exist in `scope`.

## See Also

### Creating an Attribute Container

init()

Creates an empty attribute container.

init&lt;S>([NSAttributedString.Key : Any], including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates an attribute container from a dictionary and an attribute scope that a key path identifies.

init([NSAttributedString.Key : Any])

Creates an attribute container from a dictionary, using default attribute scopes.

