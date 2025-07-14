

- Swift
- KeyedEncodingContainer
-  encodeIfPresent(\_:forKey:configuration:) 

Instance Method

# encodeIfPresent(\_:forKey:configuration:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func encodeIfPresent(
    _ t: T?,
    forKey key: KeyedEncodingContainer.Key,
    configuration: C.Type
) throws where T : EncodableWithConfiguration, C : EncodingConfigurationProviding, T.EncodingConfiguration == C.EncodingConfiguration
```

Available when `K` conforms to `CodingKey`.

