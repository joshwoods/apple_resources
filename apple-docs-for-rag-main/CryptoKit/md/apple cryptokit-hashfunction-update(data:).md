

- Apple CryptoKit
- HashFunction
-  update(data:) 

Instance Method

# update(data:)

Incrementally updates the hash function with the given data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func update(data: D) where D : DataProtocol
```

## Parameters 

`data`  

The next block of data for the ongoing digest calculation. You can provide this as any type that conforms to DataProtocol, like Data or an array of UInt8 instances.

## Discussion

Call this method one or more times to provide data to the hash function in blocks. After providing the last block of data, call the finalize() method to get the computed digest. Don’t call the update method again after finalizing the hash function.

## See Also

### Computing a hash iteratively

init()

Creates a hash function.

**Required**

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

**Required**

func finalize() -> Self.Digest

Finalizes the hash function and returns the computed digest.

**Required**

