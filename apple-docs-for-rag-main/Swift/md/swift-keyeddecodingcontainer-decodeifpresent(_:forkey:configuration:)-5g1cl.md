

- Swift
- KeyedDecodingContainer
-  decodeIfPresent(\_:forKey:configuration:) 

Instance Method

# decodeIfPresent(\_:forKey:configuration:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decodeIfPresent(
    _: T.Type,
    forKey key: KeyedDecodingContainer.Key,
    configuration: C.Type
) throws -> T? where T : DecodableWithConfiguration, C : DecodingConfigurationProviding, T.DecodingConfiguration == C.DecodingConfiguration
```

Available when `K` conforms to `CodingKey`.

