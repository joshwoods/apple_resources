

- Foundation
-  AttributeDynamicLookup 

Enumeration

# AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup @frozen
enum AttributeDynamicLookup
```

## Overview

This type allows attribute owners to add extensions that enable dynamic member lookup access to attributes. Supporting types — including AttributedString, AttributedSubstring, and AttributeContainer — gain dynamic lookup support by extending this type.

You can enable dynamic member lookup for your own AttributedStringKey attributes by defining them as implementations, collecting them into an AttributeScope and extending AttributeDynamicLookup, like in the following example:

```
public extension AttributeDynamicLookup {
    subscript(dynamicMember keyPath: KeyPath) -> T {
        return self[T.self]
    }
}
```

## Topics

### Accessing Key Values

subscript&lt;T>(T.Type) -> T

Returns an attributed string key that corresponds to a specified type.

### Accessing Framework Attribute Scopes

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.FoundationAttributes, T>) -> T

Returns the attributed string key for a specified Foundation key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.FoundationAttributes.NumberFormatAttributes, T>) -> T

Returns the attributed string key for a specified Foundation number format key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.SwiftUIAttributes, T>) -> T

Returns the attributed string key for a specified SwiftUI key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.UIKitAttributes, T>) -> T

Returns the attributed string key for a specified UIKit key path.

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.AppKitAttributes, T>) -> T

Returns the attributed string key for a specified AppKit key path.

### Subscripts

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes, T>) -> T

subscript&lt;T>(dynamicMember _: KeyPath&lt;AttributeScopes.AccessibilityAttributes, T>) -> T

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable

## See Also

### Using Defined Attributes

enum AttributeScopes

Collections of attributes that system frameworks define.

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

