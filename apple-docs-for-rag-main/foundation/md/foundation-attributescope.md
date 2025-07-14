

- Foundation
-  AttributeScope 

Protocol

# AttributeScope

A type that organizes attributes into a grouping, and supports dynamic member lookup and serialization of attribute keys.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AttributeScope : DecodingConfigurationProviding, EncodingConfigurationProviding
```

## Overview

Attribute owners — typically frameworks — define attributes with AttributedStringKey types. To allow access to attributes with dynamic member lookup, owners create one or more structures that conform to AttributeScope. The scopes provide short names for their attributes that map to the AttributedStringKey type. The following example shows how to do this:

```
struct TextStyleAttributes : AttributeScope {
    let foregroundColor : ForegroundColorAttribute // ForegroundColorAttribute.Value == Color
    let backgroundColor : BackgroundColorAttribute // BackgroundColorAttribute.Value == Color
    let underlineStyle : UnderlineStyleAttribute // UnderlineStyleAttribute.Value == UnderlineStyle
    // etc.
}
```

This allows callers to use a syntax like `myAttributedString.foregroundColor = .red`.

## Topics

### Supporting Coding Configurations

static var encodingConfiguration: AttributeScopeCodableConfiguration

The configuration for encoding the attribute scope.

**Required** Default implementation provided.

static var decodingConfiguration: AttributeScopeCodableConfiguration

The configuration for decoding the attribute scope.

**Required** Default implementation provided.

## Relationships

### Inherits From

- DecodingConfigurationProviding
- EncodingConfigurationProviding

### Conforming Types

- AttributeScopes.AccessibilityAttributes
- AttributeScopes.AppKitAttributes
- AttributeScopes.FoundationAttributes
- AttributeScopes.FoundationAttributes.NumberFormatAttributes
- AttributeScopes.SwiftUIAttributes
- AttributeScopes.UIKitAttributes

