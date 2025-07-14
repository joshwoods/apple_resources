

- Core ML
- MLMultiArray
-  withUnsafeBytes(\_:) 

Instance Method

# withUnsafeBytes(\_:)

Calls a given closure with a raw pointer to the multiarray’s storage.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func withUnsafeBytes(_ body: (UnsafeRawBufferPointer) throws -> R) rethrows -> R
```

## Parameters 

`body`  

A closure with an UnsafeRawBufferPointer parameter that points to the storage for the multiarray. This closure takes the following parameter:

`ptr`  
The pointer to the buffer.

## See Also

### Providing buffer access

func withUnsafeBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeBufferPointer&lt;S>) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s storage.

func withUnsafeMutableBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeMutableBufferPointer&lt;S>, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

func withUnsafeMutableBytes&lt;R>((UnsafeMutableRawBufferPointer, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

