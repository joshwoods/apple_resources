

- Foundation
- JSONEncoder
-  encode(\_:configuration:) 

Instance Method

# encode(\_:configuration:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func encode(
    _ value: T,
    configuration: C.Type
) throws -> Data where T : EncodableWithConfiguration, C : EncodingConfigurationProviding, T.EncodingConfiguration == C.EncodingConfiguration
```

