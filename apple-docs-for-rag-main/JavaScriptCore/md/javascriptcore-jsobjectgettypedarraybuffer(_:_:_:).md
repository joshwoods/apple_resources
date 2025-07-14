

- JavaScriptCore
-  JSObjectGetTypedArrayBuffer(\_:\_:\_:) 

Function

# JSObjectGetTypedArrayBuffer(\_:\_:\_:)

Returns the JavaScript array buffer object to use as the backing of a JavaScript typed array object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSObjectGetTypedArrayBuffer(
    _ ctx: JSContextRef!,
    _ object: JSObjectRef!,
    _ exception: UnsafeMutablePointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`object`  

The JSObjectRef with the typed array type data pointer to obtain.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A JSObjectRef with a JSTypedArrayType of kJSTypedArrayTypeArrayBuffer, or `NULL` if `object` isn’t a typed array.

## See Also

### Accessing Typed Array Information

func JSObjectGetTypedArrayBytesPtr(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> UnsafeMutableRawPointer!

Returns a temporary pointer to the backing store of a JavaScript typed array object.

func JSObjectGetTypedArrayLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteLength(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte length of a JavaScript typed array object.

func JSObjectGetTypedArrayByteOffset(JSContextRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Int

Returns the byte offset of a JavaScript typed array object.

