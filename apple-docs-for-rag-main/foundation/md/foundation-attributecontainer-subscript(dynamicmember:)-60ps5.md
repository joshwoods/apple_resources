

- Foundation
- AttributeContainer
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns a modified attribute container as part of building a chain of attributes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> AttributeContainer.Builder where K : AttributedStringKey { get }
```

## Discussion

This method returns an AttributeContainer.Builder, which allows you to chain multiple attributes in a single call, like this:

```
// An attribute container with the link and backgroundColor attributes.
let myContainer = AttributeContainer().link(myURL).backgroundColor(.yellow)
```

## See Also

### Accessing Attributes

subscript&lt;T>(T.Type) -> T.Value?

Returns the attribute that corresponds to a specified key.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns the attribute that corresponds to a specified key path.

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

Returns the attribute container that corresponds to a specified key path.

static subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes, for use as a static method.

protocol AttributedStringKey

A type that defines an attribute’s name and type.

struct Builder

A type that iteratively builds attribute containers by setting attribute values.

