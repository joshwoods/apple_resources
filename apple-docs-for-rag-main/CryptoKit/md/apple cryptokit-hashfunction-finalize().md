

- Apple CryptoKit
- HashFunction
-  finalize() 

Instance Method

# finalize()

Finalizes the hash function and returns the computed digest.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func finalize() -> Self.Digest
```

**Required**

## Return Value

The computed digest of the data.

## Discussion

Call this method after you provide the hash function with all the data to hash using one or more calls to the update(data:) or update(bufferPointer:) method. After finalizing the hash function, discard it. To compute a new digest, create a new hash function with a call to the init() method.

## See Also

### Computing a hash iteratively

init()

Creates a hash function.

**Required**

func update&lt;D>(data: D)

Incrementally updates the hash function with the given data.

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

**Required**

