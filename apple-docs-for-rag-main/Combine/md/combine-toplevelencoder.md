

- Combine
-  TopLevelEncoder 

Protocol

# TopLevelEncoder

A type that defines methods for encoding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol TopLevelEncoder
```

## Topics

### Declaring Encoder Topography

associatedtype Output

The type this encoder produces.

**Required**

### Encoding

func encode&lt;T>(T) throws -> Self.Output

Encodes an instance of the indicated type.

**Required**

## See Also

### Encoders and Decoders

protocol TopLevelDecoder

A type that defines methods for decoding.

