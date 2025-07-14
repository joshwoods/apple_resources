

- Compression
- OutputFilter
-  init(\_:using:bufferCapacity:writingTo:) 

Initializer

# init(\_:using:bufferCapacity:writingTo:)

Creates an output filter that can be used to compress or decompress data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    _ operation: FilterOperation,
    using algorithm: Algorithm,
    bufferCapacity: Int = 65536,
    writingTo writeFunc: @escaping (Data?) throws -> Void
) throws
```

