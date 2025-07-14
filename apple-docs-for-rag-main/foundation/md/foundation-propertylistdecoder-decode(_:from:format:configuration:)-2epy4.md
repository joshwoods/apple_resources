

- Foundation
- PropertyListDecoder
-  decode(\_:from:format:configuration:) 

Instance Method

# decode(\_:from:format:configuration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func decode(
    _ type: T.Type,
    from data: Data,
    format: inout PropertyListDecoder.PropertyListFormat,
    configuration: C.Type
) throws -> T where T : DecodableWithConfiguration, C : DecodingConfigurationProviding, T.DecodingConfiguration == C.DecodingConfiguration
```

