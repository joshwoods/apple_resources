

- Foundation
-  DecodableWithConfiguration 

Protocol

# DecodableWithConfiguration

A protocol for types that support decoding when supplied with an additional configuration type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol DecodableWithConfiguration
```

## Topics

### Decoding

init(from: any Decoder, configuration: Self.DecodingConfiguration) throws

Creates a new instance by retrieving the instance’s data from the specified decoder with help from the provided configuration.

**Required**

### Supporting Types

associatedtype DecodingConfiguration

The configuration type that assists in decoding.

**Required**

## Relationships

### Conforming Types

- AttributeContainer
- AttributedString
- Expression

  Conforms when `each Input` conforms to `Copyable`, `each Input` conforms to `Escapable`, `Output` conforms to `Copyable`, and `Output` conforms to `Escapable`.

- Predicate

  Conforms when `each Input` conforms to `Copyable` and `Escapable`.

## See Also

### Serializing Arbitrary Payloads

typealias CodableWithConfiguration

A type that can convert itself into and out of an external representation with the help of a configuration that handles encoding contained types.

struct CodableConfiguration

A property wrapper that makes a type codable, by supplying a configuration that provides additional information for serialization.

protocol DecodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help decode types that don’t support encoding by themselves.

protocol EncodableWithConfiguration

A protocol for types that support encoding when supplied with an additional configuration type.

protocol EncodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help encode types that don’t support encoding by themselves.

