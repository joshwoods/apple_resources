

- Compression
- InputFilter
-  init(\_:using:bufferCapacity:readingFrom:) 

Initializer

# init(\_:using:bufferCapacity:readingFrom:)

Creates an input filter that can be used to compress or decompress data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    _ operation: FilterOperation,
    using algorithm: Algorithm,
    bufferCapacity: Int = 65536,
    readingFrom readFunc: @escaping (Int) throws -> D?
) throws
```

