

- Foundation
- PropertyListEncoder
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

## See Also

### Encoding

init()

Creates a new, reusable property list encoder with the default formatting settings.

func encode&lt;Value>(Value) throws -> Data

Returns a property list that represents an encoded version of the value you supply.

func encode&lt;T>(T, configuration: T.EncodingConfiguration) throws -> Data

