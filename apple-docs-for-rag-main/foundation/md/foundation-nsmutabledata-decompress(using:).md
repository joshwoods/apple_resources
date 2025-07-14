

- Foundation
- NSMutableData
-  decompress(using:) 

Instance Method

# decompress(using:)

Decompresses the data object’s bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func decompress(using algorithm: NSData.CompressionAlgorithm) throws
```

## Parameters 

`algorithm`  

The algorithm to use for decompressing the data. For a list of available algorithms, see NSData.CompressionAlgorithm.

## Discussion

Use this method to inflate in-memory data when you need uncompressed bytes. Specify the same algorithm used to compress the data to successfully decompress it.

The following example shows how to inflate an instance of NSMutableData compressed with the NSData.CompressionAlgorithm.zlib algorithm:

```
do {
    data.decompress(using: .zlib)
} catch {
    print ("Decompression error: \(error)")
}
```

## See Also

### Compressing and Decompressing Data

func compress(using: NSData.CompressionAlgorithm) throws

Compresses the data object’s bytes using an algorithm that you specify.

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

