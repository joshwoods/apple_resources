

- Core ML
- MLMultiArray
-  withUnsafeMutableBytes(\_:) 

Instance Method

# withUnsafeMutableBytes(\_:)

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func withUnsafeMutableBytes(_ body: (UnsafeMutableRawBufferPointer, [Int]) throws -> R) rethrows -> R
```

## Parameters 

`body`  

A closure with an UnsafeMutableRawBufferPointer parameter that points to the storage for the multiarray and its strides. This closure takes the following parameters:

`ptr`  
The pointer to the buffer.

`strides`  
The strides of the buffer in scalars. Note that this may be different from `strides`’s value prior to this method invocation.

## Discussion

The buffer contains a collection of `int32`, `float16`, `float32`, or `float64` values, depending on the multiarray’s data type. It may not store these scalar values contiguously; use `strides` to get the buffer layout.

## See Also

### Providing buffer access

func withUnsafeBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeBufferPointer&lt;S>) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s storage.

func withUnsafeBytes&lt;R>((UnsafeRawBufferPointer) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s storage.

func withUnsafeMutableBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeMutableBufferPointer&lt;S>, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

