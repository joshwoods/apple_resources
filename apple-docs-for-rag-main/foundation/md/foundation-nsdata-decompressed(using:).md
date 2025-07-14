

- Foundation
- NSData
-  decompressed(using:) 

Instance Method

# decompressed(using:)

Returns a new data object by decompressing data object’s bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func decompressed(using algorithm: NSData.CompressionAlgorithm) throws -> Self
```

## Parameters 

`algorithm`  

An algorithm used to decompress the data. For a list of available algorithms, see NSData.CompressionAlgorithm.

## Return Value

An NSData instance that contains the decompressed buffer data.

## Discussion

Use this method to inflate in-memory data when you need uncompressed bytes. Specify the same algorithm used to compress the data to successfully decompress it.

The following example shows how to create a new NSData instance from data compressed with the NSData.CompressionAlgorithm.zlib algorithm:

```
do {
    let uncompressedData = try compressedData.decompressed(using: .zlib)
} catch {
    print ("Decompression error: \(error)")
}
```

## See Also

### Compressing and Decompressing Data

func compressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by compressing the data object’s bytes.

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

