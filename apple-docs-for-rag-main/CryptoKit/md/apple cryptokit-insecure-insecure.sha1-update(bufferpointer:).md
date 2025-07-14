

- Apple CryptoKit
- Insecure
- Insecure.SHA1
-  update(bufferPointer:) 

Instance Method

# update(bufferPointer:)

Incrementally updates the hash function with the contents of the buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func update(bufferPointer: UnsafeRawBufferPointer)
```

## Parameters 

`bufferPointer`  

A pointer to the next block of data for the ongoing digest calculation.

## Discussion

Call this method one or more times to provide data to the hash function in blocks. After providing the last block of data, call the finalize() method to get the computed digest. Don’t call the update method again after finalizing the hash function.

Note

Typically, it’s safer to use an instance of Data, or some other type that conforms to the DataProtocol, to hold your data. When possible, use the `update(data:)` method instead.

## See Also

### Computing a hash iteratively

init()

Creates a SHA1 hash function.

func finalize() -> Insecure.SHA1.Digest

Finalizes the hash function and returns the computed digest.

