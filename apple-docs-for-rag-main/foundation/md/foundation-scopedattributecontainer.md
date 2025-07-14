

- Foundation
-  ScopedAttributeContainer 

Structure

# ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct ScopedAttributeContainer where S : AttributeScope
```

## Overview

Use a ScopedAttributeContainer when you need to disambiguate between attributes that exist in several attribute scopes that your app uses.

## Topics

### Accessing Attribute Keys

subscript&lt;T>(dynamicMember _: KeyPath&lt;S, T>) -> T.Value?

Returns the value of the attribute that the specified key path indicates.

## Relationships

### Conforms To

- Sendable

## See Also

### Using Defined Attributes

enum AttributeScopes

Collections of attributes that system frameworks define.

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

