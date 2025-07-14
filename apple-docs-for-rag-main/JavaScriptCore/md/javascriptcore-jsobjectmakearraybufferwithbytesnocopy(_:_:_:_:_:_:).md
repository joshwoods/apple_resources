

- JavaScriptCore
-  JSObjectMakeArrayBufferWithBytesNoCopy(\_:\_:\_:\_:\_:\_:) 

Function

# JSObjectMakeArrayBufferWithBytesNoCopy(\_:\_:\_:\_:\_:\_:)

Creates a JavaScript array buffer object from an existing pointer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectMakeArrayBufferWithBytesNoCopy(
    _ ctx: JSContextRef!,
    _ bytes: UnsafeMutableRawPointer!,
    _ byteLength: Int,
    _ bytesDeallocator: JSTypedArrayBytesDeallocator!,
    _ deallocatorContext: UnsafeMutableRawPointer!,
    _ exception: UnsafeMutablePointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`bytes`  

A pointer to the byte buffer to use as the backing store of the typed array object.

`byteLength`  

The number of bytes that `bytes` points to.

`bytesDeallocator`  

The allocator to use to deallocate the external buffer when deallocating the typed array object.

`deallocatorContext`  

A pointer to pass back to the deallocator.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A JSObjectRef array buffer with a backing store that is the same as the one that `bytes` points to, or `NULL` if there is an error.

## Discussion

If the system throws an exception during this function, it always calls the `bytesDeallocator`.

## See Also

### Working with Array Buffers

func JSObjectGetArrayBufferByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the number of bytes in a JavaScript data object.

func JSObjectGetArrayBufferBytesPtr(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> UnsafeMutableRawPointer!

Returns a pointer to the data buffer that serves as the backing store for a JavaScript typed array object.

