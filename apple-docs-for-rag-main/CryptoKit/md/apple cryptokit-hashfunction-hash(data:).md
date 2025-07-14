

- Apple CryptoKit
- HashFunction
-  hash(data:) 

Type Method

# hash(data:)

Computes the digest of the bytes in the given data instance and returns the computed digest.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func hash(data: D) -> Self.Digest where D : DataProtocol
```

## Parameters 

`data`  

The data whose digest the hash function should compute. This can be any type that conforms to DataProtocol, like Data or an array of UInt8 instances.

## Return Value

The computed digest of the data.

## Discussion

Use this method if all your data fits into a single data instance. If the data you want to hash is too large, initialize a hash function and use the update(data:) and finalize() methods to compute the digest in blocks.

