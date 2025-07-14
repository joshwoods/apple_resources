

- Foundation
- AttributeDynamicLookup
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns the attributed string key for a specified Foundation number format key path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> T where T : AttributedStringKey { get }
```

## See Also

### Accessing Framework Attribute Scopes

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.FoundationAttributes, T>) -> T

Returns the attributed string key for a specified Foundation key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.SwiftUIAttributes, T>) -> T

Returns the attributed string key for a specified SwiftUI key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.UIKitAttributes, T>) -> T

Returns the attributed string key for a specified UIKit key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.AppKitAttributes, T>) -> T

Returns the attributed string key for a specified AppKit key path.

