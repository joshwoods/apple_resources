

- Foundation
- AttributeContainer
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns the attribute container that corresponds to a specified key path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> ScopedAttributeContainer where S : AttributeScope { get set }
```

## Discussion

Use this subscript when you need to work with an explicit attribute scope. For example, the SwiftUI foregroundColor attribute overrides the attribute in the AppKit and UIKit scopes with the same name. If you work with both the SwiftUI and UIKit scopes, you can use the syntax `myAttributeContainer.uiKit.foregroundColor` to disambiguate and explicitly use the UIKit attribute.

## See Also

### Accessing Attributes

subscript&lt;T>(T.Type) -> T.Value?

Returns the attribute that corresponds to a specified key.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns the attribute that corresponds to a specified key path.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes.

static subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes, for use as a static method.

protocol AttributedStringKey

A type that defines an attribute’s name and type.

struct Builder

A type that iteratively builds attribute containers by setting attribute values.

