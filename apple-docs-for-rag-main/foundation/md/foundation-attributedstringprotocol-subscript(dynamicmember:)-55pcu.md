

- Foundation
- AttributedStringProtocol
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns a scoped attribute container that a key path indicates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> ScopedAttributeContainer where S : AttributeScope { get set }
```

**Required**

## Discussion

Use this subscript when you need to work with an explicit attribute scope. For example, the SwiftUI foregroundColor attribute overrides the attribute in the AppKit and UIKit scopes with the same name. If you work with both the SwiftUI and UIKit scopes, you can use the syntax `myAttributedString.uiKit.foregroundColor` to disambiguate and explicitly use the UIKit attribute.

The attribute container that this method returns contains only attributes that exist, and are present and identical for the entire attributed string. To find portions of the string with consistent attributes, use the `AttributedString/runs` property.

Getting or setting stringwide attributes with this subscript has `O(n)` behavior in the worst case, where `n` is the number of runs.

## See Also

### Accessing Whole-String Attributes

subscript&lt;K>(K.Type) -> K.Value?

Returns an attribute value that corresponds to an attributed string key.

**Required**

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns an attribute value that a key path indicates.

**Required**

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

