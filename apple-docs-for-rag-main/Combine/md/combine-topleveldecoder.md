

- Combine
-  TopLevelDecoder 

Protocol

# TopLevelDecoder

A type that defines methods for decoding.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol TopLevelDecoder
```

## Topics

### Declaring Encoder Topography

associatedtype Input

The type this decoder accepts.

**Required**

### Decoding

func decode&lt;T>(T.Type, from: Self.Input) throws -> T

Decodes an instance of the indicated type.

**Required**

## See Also

### Encoders and Decoders

protocol TopLevelEncoder

A type that defines methods for encoding.

