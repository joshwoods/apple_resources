

- Accelerate
- AccelerateBuffer
-  withUnsafeBufferPointer(\_:) 

Instance Method

# withUnsafeBufferPointer(\_:)

Calls a closure with a pointer to the object’s contiguous storage.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func withUnsafeBufferPointer(_ body: (UnsafeBufferPointer) throws -> R) rethrows -> R
```

**Required** Default implementation provided.

## Parameters 

`body`  

A closure that receives an UnsafeBufferPointer to the sequence’s contiguous storage.

## Default Implementations

### AccelerateBuffer Implementations

func withUnsafeBufferPointer&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R

