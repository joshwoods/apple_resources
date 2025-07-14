

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
    configuration: T.EncodingConfiguration
) throws where T : EncodableWithConfiguration
```

Available when `K` conforms to `CodingKey`.

