

- JavaScriptCore
-  JSObjectGetArrayBufferBytesPtr(\_:\_:\_:) 

Function

# JSObjectGetArrayBufferBytesPtr(\_:\_:\_:)

Returns a pointer to the data buffer that serves as the backing store for a JavaScript typed array object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectGetArrayBufferBytesPtr(
    _ ctx: JSContextRef!,
    _ object: JSObjectRef!,
    _ exception: UnsafeMutablePointer!
) -> UnsafeMutableRawPointer!
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef with the typed array type data pointer to obtain.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Discussion

The pointer that this function returns is temporary and may not remain valid across JavaScriptCore API calls.

## See Also

### Working with Array Buffers

func JSObjectMakeArrayBufferWithBytesNoCopy(JSContextRef!, UnsafeMutableRawPointer!, Int, JSTypedArrayBytesDeallocator!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Creates a JavaScript array buffer object from an existing pointer.

func JSObjectGetArrayBufferByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the number of bytes in a JavaScript data object.

