

- Foundation
- JSONDecoder
-  decode(\_:from:configuration:) 

Instance Method

# decode(\_:from:configuration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func decode(
    _ type: T.Type,
    from data: Data,
    configuration: C.Type
) throws -> T where T : DecodableWithConfiguration, C : DecodingConfigurationProviding, T.DecodingConfiguration == C.DecodingConfiguration
```

