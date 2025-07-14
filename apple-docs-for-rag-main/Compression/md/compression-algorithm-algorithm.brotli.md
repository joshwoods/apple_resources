

- Compression
- Algorithm
-  Algorithm.brotli 

Case

# Algorithm.brotli

The Brotli compression algorithm, which is recommended for text compression.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case brotli
```

## Discussion

The Brotli compression algorithm is a widely adopted content encoding method for the web. The Compression framework includes Brotli to provide decoding capabilities.

The Compression framework implements the Brotli level 2 encoder only. This compression level provides a good balance between compression speed and compression ratio. The Brotli decoder supports decoding data compressed with any compression level.

