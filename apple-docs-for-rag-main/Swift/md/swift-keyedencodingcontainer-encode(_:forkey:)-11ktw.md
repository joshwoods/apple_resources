

- Swift
- KeyedEncodingContainer
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func encode(
    _ wrapper: CodableConfiguration,
    forKey key: KeyedEncodingContainer.Key
) throws where T : DecodableWithConfiguration, T : EncodableWithConfiguration, C : DecodingConfigurationProviding, C : EncodingConfigurationProviding, T.DecodingConfiguration == C.DecodingConfiguration, T.EncodingConfiguration == C.EncodingConfiguration
```

Available when `K` conforms to `CodingKey`.

