

- Foundation
- AttributedString
-  init(\_:including:) 

Initializer

# init(\_:including:)

Creates a value-type attributed string from a reference type, including an attribute scope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ nsStr: NSAttributedString,
    including scope: S.Type
) throws where S : AttributeScope
```

## Parameters 

`nsStr`  

The NSAttributedString to convert.

`scope`  

The attribute scope of the attributes in `nsStr`. This can be a nested scope that contains several scopes.

## Discussion

This initializer only collects attributes from `nsStr` that exist in the provided scope. The resulting attributed string omits any keys in `nsStr` that don’t exist in `scope`.

## See Also

### Creating an Attributed String from a Reference Type

init&lt;S>(NSAttributedString, including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates a value-type attributed string from a reference type, including an attribute scope that a key path identifies.

init(NSAttributedString)

Creates a value-type attributed string from a reference type.

