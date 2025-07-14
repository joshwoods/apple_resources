

- Foundation
- NSMutableData
-  compress(using:) 

Instance Method

# compress(using:)

Compresses the data object’s bytes using an algorithm that you specify.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func compress(using algorithm: NSData.CompressionAlgorithm) throws
```

## Parameters 

`algorithm`  

The algorithm to use to compress the data. For a list of available algorithms, see NSData.CompressionAlgorithm.

## Discussion

Use this method to compress in-memory data when you want to reduce memory usage and can afford the time to compress and decompress the data. If your data object is already in a compressed format, such as media formats like JPEG images or AAC audio, compress(using:) may provide minimal or no benefit.

The following example shows how to compress data from a string and prints the sizes of the data instances to illustrate the amount of compression:

```
var string = "NSData and its mutable subclass NSMutableData provide data objects, or object-oriented wrappers for byte buffers. Data objects let simple allocated buffers (that is, data with no embedded pointers) take on the behavior of Foundation objects."
let data = NSMutableData(data: Data(string.utf8))
print ("original data size: \(data.length)")
do {
    try data.compress(using: .zlib)
    print("zlib compressed size: \(data.length)")
} catch {
    print ("Compression error: \(error)")
}
// Prints:
//  original data size: 241
//  zlib compressed size: 158
```

## See Also

### Compressing and Decompressing Data

func decompress(using: NSData.CompressionAlgorithm) throws

Decompresses the data object’s bytes.

enum CompressionAlgorithm

An algorithm that indicates how to compress or decompress data.

var NSCompressionErrorMaximum: Int

The end of the range of error codes reserved for compression errors.

var NSCompressionErrorMinimum: Int

The start of the range of error codes reserved for compression errors.

var NSCompressionFailedError: Int

An error code value that indicates a failure to compress data using the provided algorithm.

var NSDecompressionFailedError: Int

An error code value that indicates a failure to decompress data using the provided algorithm.

