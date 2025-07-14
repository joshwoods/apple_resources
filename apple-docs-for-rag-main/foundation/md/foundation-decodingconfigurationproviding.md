

- Foundation
-  DecodingConfigurationProviding 

Protocol

# DecodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help decode types that don’t support encoding by themselves.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol DecodingConfigurationProviding
```

## Topics

### Accessing the Configuration

static var decodingConfiguration: Self.DecodingConfiguration

The configuration instance that assists in decoding another type.

**Required** Default implementation provided.

### Supporting Types

associatedtype DecodingConfiguration

**Required**

## Relationships

### Inherited By

- AttributeScope

### Conforming Types

- AttributeScopes.AccessibilityAttributes
- AttributeScopes.AppKitAttributes
- AttributeScopes.FoundationAttributes
- AttributeScopes.FoundationAttributes.NumberFormatAttributes
- AttributeScopes.SwiftUIAttributes
- AttributeScopes.UIKitAttributes

## See Also

### Serializing Arbitrary Payloads

typealias CodableWithConfiguration

A type that can convert itself into and out of an external representation with the help of a configuration that handles encoding contained types.

struct CodableConfiguration

A property wrapper that makes a type codable, by supplying a configuration that provides additional information for serialization.

protocol DecodableWithConfiguration

A protocol for types that support decoding when supplied with an additional configuration type.

protocol EncodableWithConfiguration

A protocol for types that support encoding when supplied with an additional configuration type.

protocol EncodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help encode types that don’t support encoding by themselves.

