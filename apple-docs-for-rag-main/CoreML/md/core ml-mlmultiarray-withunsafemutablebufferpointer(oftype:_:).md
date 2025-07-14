

- Core ML
- MLMultiArray
-  withUnsafeMutableBufferPointer(ofType:\_:) 

Instance Method

# withUnsafeMutableBufferPointer(ofType:\_:)

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func withUnsafeMutableBufferPointer(
    ofType type: S.Type,
    _ body: (UnsafeMutableBufferPointer, [Int]) throws -> R
) rethrows -> R where S : MLShapedArrayScalar
```

## Parameters 

`type`  

The element type of the buffer passed in the body. This must be a Swift primitive type equivalent to `dataType`.

`body`  

A closure with an UnsafeMutableBufferPointer parameter that points to the storage for the multiarray and its strides. This closure takes the following parameters:

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

func withUnsafeMutableBytes&lt;R>((UnsafeMutableRawBufferPointer, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

