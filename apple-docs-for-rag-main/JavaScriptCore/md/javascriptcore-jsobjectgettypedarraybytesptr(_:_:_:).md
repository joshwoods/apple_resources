

- JavaScriptCore
-  JSObjectGetTypedArrayBytesPtr(\_:\_:\_:) 

Function

# JSObjectGetTypedArrayBytesPtr(\_:\_:\_:)

Returns a temporary pointer to the backing store of a JavaScript typed array object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectGetTypedArrayBytesPtr(
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

## Return Value

The pointer that this function returns is temporary and may not remain valid across JavaScriptCore API calls.

## See Also

### Accessing Typed Array Information

func JSObjectGetTypedArrayLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteOffset(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte offset of a JavaScript typed array object.

func JSObjectGetTypedArrayBuffer(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Returns the JavaScript array buffer object to use as the backing of a JavaScript typed array object.

