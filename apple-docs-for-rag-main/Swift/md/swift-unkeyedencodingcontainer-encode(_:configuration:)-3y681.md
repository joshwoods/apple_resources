

- Swift
- UnkeyedEncodingContainer
-  encode(\_:configuration:) 

Instance Method

# encode(\_:configuration:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func encode(
    _ t: T,
    configuration: C.Type
) throws where T : EncodableWithConfiguration, C : EncodingConfigurationProviding, T.EncodingConfiguration == C.EncodingConfiguration
```

