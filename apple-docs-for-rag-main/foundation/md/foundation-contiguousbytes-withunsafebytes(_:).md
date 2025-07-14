

- Foundation
- ContiguousBytes
-  withUnsafeBytes(\_:) 

Instance Method

# withUnsafeBytes(\_:)

Calls the given closure with a pointer to the underlying bytes of the type’s contiguous storage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafeBytes(_ body: (UnsafeRawBufferPointer) throws -> R) rethrows -> R
```

**Required**

## Parameters 

`body`  

A closure with an UnsafeRawBufferPointer parameter that points to the contiguous storage for the type. If no such storage exists, the method creates it. If `body` has a return value, this method also returns that value. The argument is valid only for the duration of the closure’s execution.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

The following example copies the bytes from a string encoded using `utf8` into a buffer of `UInt8`:

```
let data = "Hello".data(using: .utf8)
var byteBuffer: [UInt8] = []
_ = data?.withUnsafeBytes { buffer in
    byteBuffer.append(contentsOf: buffer)
}

// byteBuffer = [72, 101, 108, 108, 111]
```

