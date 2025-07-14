

- Apple CryptoKit
- HashFunction
-  init() 

Initializer

# init()

Creates a hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

**Required**

## Discussion

Initialize a new hash function by calling this method if you want to hash the data iteratively, such as when you don’t have a buffer large enough to hold all the data at once. Provide data blocks to the hash function using the update(data:) or update(bufferPointer:) method. After providing all the data, call finalize() to get the digest.

If your data fits into a single buffer, you can use the hash(data:) method instead to compute the digest in a single call.

## See Also

### Computing a hash iteratively

func update&lt;D>(data: D)

Incrementally updates the hash function with the given data.

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

**Required**

func finalize() -> Self.Digest

Finalizes the hash function and returns the computed digest.

**Required**

