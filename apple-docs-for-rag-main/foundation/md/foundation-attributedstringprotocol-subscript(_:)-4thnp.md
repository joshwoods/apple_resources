

- Foundation
- AttributedStringProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns an attribute value that corresponds to an attributed string key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(_: K.Type) -> K.Value? where K : AttributedStringKey, K.Value : Sendable { get set }
```

**Required**

## Discussion

This subscript returns `nil` unless the specified attribute exists, and is present and identical for the entire attributed string or substring. To find portions of an attributed string with consistent attributes, use the `AttributedString/runs` property.

Getting or setting stringwide attributes with this subscript has `O(n)` behavior in the worst case, where `n` is the number of runs.

## See Also

### Accessing Whole-String Attributes

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns an attribute value that a key path indicates.

**Required**

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

Returns a scoped attribute container that a key path indicates.

**Required**

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

