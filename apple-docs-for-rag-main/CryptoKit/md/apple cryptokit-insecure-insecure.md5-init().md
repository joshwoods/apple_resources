

- Apple CryptoKit
- Insecure
- Insecure.MD5
-  init() 

Initializer

# init()

Creates a MD5 hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

## Discussion

Initialize a new hash function by calling this method if you want to hash the data iteratively, such as when you don’t have a buffer large enough to hold all the data at once. Provide data blocks to the hash function using the `update(data:)` or update(bufferPointer:) method. After providing all the data, call finalize() to get the digest.

If your data fits into a single buffer, you can use the `hash(data:)` method instead, to compute the digest in a single call.

## See Also

### Computing a hash iteratively

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

func finalize() -> Insecure.MD5.Digest

Finalizes the hash function and returns the computed digest.

