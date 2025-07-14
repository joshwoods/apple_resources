

- JavaScriptCore
-  JSObjectGetArrayBufferByteLength(\_:\_:\_:) 

Function

# JSObjectGetArrayBufferByteLength(\_:\_:\_:)

Returns the number of bytes in a JavaScript data object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectGetArrayBufferByteLength(
    _ ctx: JSContextRef!,
    _ object: JSObjectRef!,
    _ exception: UnsafeMutablePointer!
) -> Int
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JavaScript array buffer object with the length in bytes to return.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

The number of bytes in the data object.

## See Also

### Working with Array Buffers

func JSObjectMakeArrayBufferWithBytesNoCopy(JSContextRef!, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array buffer object from an existing pointer.

func JSObjectGetArrayBufferBytesPtr(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> UnsafeMutableRawPointer!

Returns a pointer to the data buffer that serves as the backing store for a JavaScript typed array object.

