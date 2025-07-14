

- Swift
- KeyedDecodingContainer
-  decode(\_:forKey:) 

Instance Method

# decode(\_:forKey:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decode(
    _: CodableConfiguration.Type,
    forKey key: KeyedDecodingContainer.Key
) throws -> CodableConfiguration where T : DecodableWithConfiguration, T : EncodableWithConfiguration, C : DecodingConfigurationProviding, C : EncodingConfigurationProviding, T.DecodingConfiguration == C.DecodingConfiguration, T.EncodingConfiguration == C.EncodingConfiguration
```

Available when `K` conforms to `CodingKey`.

