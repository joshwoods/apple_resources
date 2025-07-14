

- Apple CryptoKit
- Insecure
- Insecure.MD5
-  finalize() 

Instance Method

# finalize()

Finalizes the hash function and returns the computed digest.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func finalize() -> Insecure.MD5.Digest
```

## Return Value

The computed digest of the data.

## Discussion

Call this method after you provide the hash function with all the data to hash by making one or more calls to the `update(data:)` or update(bufferPointer:) method. After finalizing the hash function, discard it. To compute a new digest, create a new hash function with a call to the init() method.

## See Also

### Computing a hash iteratively

init()

Creates a MD5 hash function.

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

