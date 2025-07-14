

- Accelerate
- AccelerateMutableBuffer
-  withUnsafeMutableBufferPointer(\_:) 

Instance Method

# withUnsafeMutableBufferPointer(\_:)

Calls the given closure with a pointer to the object’s mutable contiguous storage.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
mutating func withUnsafeMutableBufferPointer(_ body: (inout UnsafeMutableBufferPointer) throws -> R) rethrows -> R
```

**Required** Default implementation provided.

## Parameters 

`body`  

A closure that receives an UnsafeMutableBufferPointer to the sequence’s contiguous storage.

## Default Implementations

### AccelerateMutableBuffer Implementations

func withUnsafeMutableBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

