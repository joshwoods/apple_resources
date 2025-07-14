

- Foundation
- EncodableWithConfiguration
-  encode(to:configuration:) 

Instance Method

# encode(to:configuration:)

Encodes the value into the specified encoder with help from the provided configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func encode(
    to encoder: any Encoder,
    configuration: Self.EncodingConfiguration
) throws
```

**Required**

## Parameters 

`encoder`  

The encoder to write data to.

`configuration`  

An encoding configuration instance that provides additional information necessary for encoding.

