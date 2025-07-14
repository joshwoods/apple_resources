

- Foundation
-  AttributeScopes 

Enumeration

# AttributeScopes

Collections of attributes that system frameworks define.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum AttributeScopes
```

## Overview

Attribute scopes define groups of attributes appropriate for use with attributed strings in a certain domain. Attribute definitions contain a name, value type, and encode/decode methods to support serialization.

For example, the AttributeScopes.FoundationAttributes scope provides an attribute type for a link to a URL, AttributeScopes.FoundationAttributes.LinkAttribute, along with a property to access this type, link. Because AttributeScopes.FoundationAttributes implements AttributeDynamicLookup, you can access the link attribute by name, as this example shows:

```
var attrStr = AttributedString("Example site")
attrStr.link = URL(string: "http://example.com")
```

## Topics

### Foundation-Defined Attributes

var foundation: AttributeScopes.FoundationAttributes.Type

A property for accessing the attribute scopes that Foundation defines.

struct FoundationAttributes

Attribute scopes that Foundation defines.

### SwiftUI-Defined Attributes

var swiftUI: AttributeScopes.SwiftUIAttributes.Type

A property for accessing the attribute scopes that SwiftUI defines.

struct SwiftUIAttributes

Attribute scopes that SwiftUI defines.

### UIKit-Defined Attributes

var uiKit: AttributeScopes.UIKitAttributes.Type

A property for accessing the attribute scopes that UIKit defines.

struct UIKitAttributes

Attribute scopes that UIKit defines.

### AppKit-Defined Attributes

var appKit: AttributeScopes.AppKitAttributes.Type

A property for accessing the attribute scopes that AppKit defines.

struct AppKitAttributes

Attribute scopes that AppKit defines.

### Structures

struct AccessibilityAttributes

### Instance Properties

var accessibility: AttributeScopes.AccessibilityAttributes.Type

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable

## See Also

### Using Defined Attributes

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

