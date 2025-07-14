

- Foundation
-  CodableWithConfiguration 

Type Alias

# CodableWithConfiguration

A type that can convert itself into and out of an external representation with the help of a configuration that handles encoding contained types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias CodableWithConfiguration = DecodableWithConfiguration & EncodableWithConfiguration
```

## Discussion

CodableWithConfiguration is a type alias for the EncodableWithConfiguration and DecodableWithConfiguration protocols. Use this protocol to support codability in a type that can’t conform to Codable by itself, but can do so with additional statically-defined configuration provided by a CodableConfiguration instance.

AttributedString uses this approach to allow an instance to contain arbitrary attributes, including frameworks outside of Foundation or the platform SDK. It does this by including one or more AttributeScope instances, a type that conforms to EncodingConfigurationProviding and DecodingConfigurationProviding. An attribute scope like AttributeScopes.SwiftUIAttributes defines attribute keys, and conforms to AttributeScope to provide configuration instances that know the AttributedStringKey types and their associated Value types. With this type information, an AttributedString can encode all of its attributes, even from frameworks other than Foundation.

## See Also

### Serializing Arbitrary Payloads

struct CodableConfiguration

A property wrapper that makes a type codable, by supplying a configuration that provides additional information for serialization.

protocol DecodableWithConfiguration

A protocol for types that support decoding when supplied with an additional configuration type.

protocol DecodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help decode types that don’t support encoding by themselves.

protocol EncodableWithConfiguration

A protocol for types that support encoding when supplied with an additional configuration type.

protocol EncodingConfigurationProviding

A protocol whose conformers provide a configuration instance to help encode types that don’t support encoding by themselves.

